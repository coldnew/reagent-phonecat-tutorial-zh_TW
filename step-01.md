# Step-01: 顯示靜態內容

**[Browse code](https://github.com/vvvvalvalval/reagent-phonecat-tutorial/blob/step-1/src/cljs/reagent_phonecat_tutorial/core.cljs#L1) - [Diff](https://github.com/vvvvalvalval/reagent-phonecat-tutorial/compare/step-0...step-1#diff-0bf18c482292a447479e4cfbf8a64631)- [Live demo](http://reagent-phonecat-tutorial.s3-website-us-east-1.amazonaws.com/step-01/)**

在測試這一份教學的步驟，你需要執行 `git checkout step-1`, 然後重新整理瀏覽器。

***

為了可以熟悉 Reagent 語法來建立不同的顯示畫面，讓我們將一些靜態內容加入到我們的網頁。 `reagent-phonecat.core` 這個命名空間的內容將變成:

```clojure
(def static-content "Some sample, statically defined DOM content."
  [:ul#phones-list
   [:li.phone-item
    [:span "Nexus S"]
    [:p "Fast just got faster with Nexus S"]]
   [:li {:class "phone-item"}
    [:span "Motorola XOOM™ with Wi-Fi"]
    [:p "The Next, Next Generation tablet."]]
   ])
```

```clojure
(defn mount-root "Creates the application view and injects ('mounts') it into the root element."
  []
  (rg/render
    static-content
    (.getElementById js/document "app")))

(defn init! []
  (mount-root))
```

如果你曾經用過 Hiccup 來建立伺服器端的 HTML樣板，你會覺得這很像，如果沒有的話，你可能需要一些時間來熟悉這個語法。

- HTML 元素將以陣列 (vector) 的形式來表示，並且第一個元素是 關鍵字 (keyword)
- HTML 屬性則是在陣列 (vector) 的第二個元素，以 map 來表示
- 在關鍵字 (keyword) 內的 `id` 和 `class` 屬性也有縮寫可以用


## 總結