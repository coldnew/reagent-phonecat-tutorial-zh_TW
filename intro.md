# 前言
本篇翻譯自: https://github.com/vvvvalvalval/reagent-phonecat-tutorial/wiki

在這份教學中，我們將透過[ClojureScript](https://clojurescript.org) 以及 [Reagent](https://reagent-project.github.io) 這個 ClojureScript 對於 Facebook 的 [React](http://facebook.github.io/react/) 函式庫的封裝，來建立一個網頁程式。

這份教學是基於 AnuglarJS 官方的 [Phonecat Tutorial](https://docs.angularjs.org/tutorial) 產生的。

## 這個專案

我們將一步一步的建立一個線上的手機型錄。你可以在 [這邊](http://reagent-phonecat-tutorial.s3-website-us-east-1.amazonaws.com/step-11/#/phones) 看到最終的成果。


這種我們將建立的網站又稱為 "單頁面應用程式"([Single Page Application, SPA](https://en.wikipedia.org/wiki/Single-page_application))。
在單頁面應用程式(SPA)下，瀏覽器只會載入一個HTML檔案，當Javascript透過伺服器更新新的資料並修改修改DOM樹後，使用者看到的就像是不同頁面在切換一樣，這種模式和傳統的網站每次使用者瀏覽新的頁面時，瀏覽器就必須載入HTML檔案的狀況不同。

單頁面應用程式(SPA)提供無縫且非常流暢的使用者體驗，但也帶來了許多挑戰，因為這種模式需要很複雜的狀態管理，這也是ClojureScript和React的語法可勝任的部份。

## 預先準備

這份教學假設你:

- 稍微理解 Clojure(Script) 的語法，如果不會的話，這份 [ClojureScript和Javascript對照表](https://himera.herokuapp.com/synonym.html) 也許對你有些幫助，或是這個 [cheatsheet](http://cljs.info/cheatsheet/)。

- 理解基本的瀏覽器運作流程(HTML、CSS、Javascript、AJAX、非同步...等)。

- 看過 [Reagent 首頁](https://reagent-project.github.io/) 可能對你有些幫助。

- 具有Reactjs相關的知識也許會有幫助，但那不是必備的。(作者在用Reagent寫app之前完全不會Reactjs)。


在做這份教學時，你 *不需要* 做過原本的 [Angular 教學](https://docs.angularjs.org/tutorial/step_00) 。

## 讓我們開始吧

準備好要開始了嘛? 請[往這邊走](https://github.com/clojure-tw/reagent-phonecat-tutorial-zh_TW/blob/master/step-00.md)。
