# OBS multi-function clock

## 概覽 Overview
這是寫來用在OBS(或Streamlabs OBS)的簡易時鐘，具有倒數計時的功能，基於[moment.js](https://momentjs.com/)及[SAM大](https://github.com/sam0737)的[作品](https://gist.github.com/sam0737/a0ee8ca253fc5c84b2aa2ac018f7b8ad)，使用時無須安裝任何插件，僅需利用瀏覽器來源便可達成，可透過Query調整模式、樣式。

A simple clock with countdown function designed for OBS and Streamlabs OBS without installin. No other softwares and plugins are needed. And user can change its mode or add custom style by Query strings.

## 參數 Parameter
在網址後輸入`?`並輸入各項所需參數，各參數間以`&`連接。
例如`網址?mode=clock&style=color: red`。

Add `?` then input parameters after the URL, and connect parameters by `&`.<br />
e.g. `URL?mode=clock&style=color: red`.
### 通用 General
- 使用 `mode` 調整模式，若未指定模式則預設為時鐘模式。<br />Use `mode` to set the mode of clock. Default mode is clock mode.
- 使用 `style` 加入CSS代碼變更字體樣式。<br />Use `style` to add more style to the output element.
- 使用 `bodyStyle` 加入CSS代碼變更背景樣式。<br />Use `bodyStyle` for the style to the body element.

### 時鐘模式 Clock Mode
使用 `mode=clock` 參數或不使用 `mode` 參數可進入時鐘模式。<br />Use `mode=clock` or not input `mode` parameter can enter clock mode.
- 使用 `format` 調整日期及時間格式。<br />Use `format` to control the date format.
- 時鐘模式其他詳細參數，請參照https://momentjs.com/docs/#/displaying/format/<br />For more detail syntax, see https://momentjs.com/docs/#/displaying/format/

### 倒數計時器模式 Countdown Timer Mode
使用 `mode=timer` 參數可進入倒數計時器模式。<br />Use `mode=timer` can enter clock mode.
- 使用 `time` 設置倒數時間，單位為秒。<br />Use `time` to set timer in the unit of second.
- 或使用 `hour` `min` `sec` 來設置不同單位的倒數時間。<br />Or use `hour` `min` `sec` to set timer in different unit.
- 使用 `msg` 來設置倒數結束後顯示的文字。<br />Use `msg` to set text that displayed after time is on.

## 例子 Examples
請參考這個[專案](https://gist.github.com/sam0737/a0ee8ca253fc5c84b2aa2ac018f7b8ad)。<br />
You can refer this [repository](https://gist.github.com/sam0737/a0ee8ca253fc5c84b2aa2ac018f7b8ad) for examples.

## 授權 License
本專案使用MIT授權。<br />
This software is licensed under the MIT License.
