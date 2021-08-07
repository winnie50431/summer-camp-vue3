# summer-camp-vue3


## 【Week1 資料卡】
> 作業目標: Lv1 **套用版型並新增功能**
##### _功能_
1. 一鍵切換頭像解析度
2. 呈現 data
3. 選取喜好項目；雙擊取消選取

##### _Note_
- `{{}}` 顯示物件
- `v-if` & `v-else` 使用
- `v-for` 遍歷提取陣列資料
- `v-on` 監聽事件
- `v-bind` `欲綁定的連結${itemName}`

## 【Week2 計算機】

> 作業目標: Lv2 **將記錄儲存到localstorage，並保持最多10筆紀錄。**  

##### _Note_
**生命週期**
- 每個Vue的元件從建立-掛載-更新-銷毀移除 的過程。

**Composition API** (Vue 3.0)  
- 兼容Vue 2.x/3.x的 Hooks function。
- Vue.js提供callback function，在週期的各個階段執行對應處理。這些callback function被稱作生命週期的Hooks function。


## 【Week3 TodoList】

> 作業目標: Lv3 **自創版型並完成過濾功能** (8.8更新 照著作業要求的功能，重新製作上傳)

_Note_
- DOM 的更新動作在 Vue.js 裡是非同步執行的，
- `created()` - 直到 Vue 實體內的各種屬性、狀態的偵測 ( `getter` 與 `setter` ) 都已經初始化完成後，才進入`created()`階段。 ( 如需透過遠端 API 來取得資料，至少得在 created 階段以後才能存取實體的 data 屬性。 ) 
- `mounted()` - 直到 `mounted()` 階段， Vue.js 才正式將網頁上的 DOM 節點、事件都綁定至 Vue 的實體。
- `watch:`屬性 - 當`data`被更新時觸發。 

參考資料: [元件的生命週期與更新機制](https://book.vue.tw/CH1/1-7-lifecycle.html)
| Hooks 名稱(Vue 2.x/3.x) | Hooks 名稱(Vue 3.0 Composition API) | 說明 |
| :-- | :-- |:--|
| `created` | `setup()` | 實體建立階段: 狀態與事件已初始化完成 (prop、data、computed 等屬性已建立，vm.$el 屬性無法使用 ) |
| `mounted` | `onMounted` | 實體建立階段: Vue 實體與掛載完成， el 的目標 DOM 被 $el 所替換。 (可以視作 jQuery 的 Ready)|

