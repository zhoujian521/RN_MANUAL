# React-Native 开发手册

## 技术栈
01. `iOS => OC`
02. `Android => java`
01. `js=>jsx` / `ts=>tsx`
02. 路由管理

    [react-navigation](https://www.npmjs.com/search?q=react-navigation)

    [ReactNative 建议使用](https://reactnative.cn/docs/navigation#__docusaurus)

    ```
        react-navigation-stack
        react-navigation-hooks
        react-navigation-tabs
    ```
    [react-native-router-flux](https://www.npmjs.com/search?q=react-native-router-flux)
    ```
        react-native-router-flux
    ```

03. 数据流管理

    [redux](https://github.com/reduxjs/redux)
    ```
        react-redux
        redux-actions
        redux-persist
        redux-saga
        reselect
    ```
    [mobx](https://github.com/mobxjs/mobx)
    ```
        mobx-react
    ```
## Git 提交规范
---

### 01：版本控制

![GitFlow](https://upload-images.jianshu.io/upload_images/5901013-dafff7b4d41716fa.png?imageMogr2/auto-orient/strip|imageView2/2/format/webp "GitFlow 流程控制")

> git 版本控制

1. master: `分支存放所有正式发布的版本，可以作为项目历史版本记录分支，不直接提交代码。`
2. develop `分支为主开发分支。`
3. feature/fun `分支为主开发分支。`
4. v1.0.0 `release版本` => `tag 标识`

### 02：Commit Rules

> 01：fun [Commit message 和 Change log 编写指南](http://www.ruanyifeng.com/blog/2016/01/commit_message_change_log.html)

> 02：task

- Commit Rules
  - part1: [Categoty]
  - part2: #SW-CardNumber
  - part3: comment

- Category
  - T: Task
  - F: Feature
  - B: Bug

- commit && push
  - husky


## 项目结构

---
1. __tests__
2. android
3. App/src
4. ios
5. node_modules
6. Tests
> .babelrc`babel的配置文件`      
> .buckconfig
> .eslintrc.js `eslint+prettier+editorconfig`      
> .editorconfig `eslint+prettier+editorconfig`      
> .flowconfig `静态文件类型检查`      
> .gitattributes      
> .gitignore      
> .prettierrc.js`eslint+prettier+editorconfig`      
> watchmanconfig `监控文件变化=>所见即所得的目的`      
> app.json     
> babel.config.js     
> index.js     
> metro.config.js` ==> 0.59 => 按需加载`     
> package.json     
> README.md     
> yarn.lock

### 01：RN
> api/service      
> assets      
    >> fonts       
    >> images    

> components`=>组件命名、组件导出`  
> constants    
> hooks      
> navigators      
> sagas      
> screens/page      
> store      
    >> qwer      
        >>> index.js      
        >>> QwerAction.js      
        >>> QwerReducers.js      

> theme      
    >> Colors.js      
    >> Fonts.js      
    >> Images.js      
    >> index.js      
    >> Metrics.js      

> utils      
> App.js      

### 02：iOS

1. MyAppNames
    01. AppDelegate
    02. Modules
        001. RCTZoom
    03. Frameworks
        001. MobileRTC.framework
        002. MobileRTCScreenShare.framework
        003. IQKeyboardManager
        004. Zoom
                * SDKPresenters
                * CustomMeeting
    04. Assets.xcassets
    05. Info.plist
    06. main.m
    07. ......
2. Resources (资源型文件目录)
    01. images 
    02. plist 
3. Frameworks `使用cocoaPods 会自动创建`

### 03：Android
`待定`

## 编程规约
---

### 01：iOS  
`待定`

### 02：Android 
`待定`

### 03：RN

1. 命名规范 
   01. 文件 
   ```
        001：文件夹
        002：jsx 文件
        003：js 文件
   ```
   02. component
        >PlanAAA      
        >>index.js     
        >>ComponentA.jsx      
        >>ComponentB.jsx      

        >PlanBBB      
        >> ComponentA
        >>> index.jsx      

        >> ComponentB      
            >>> index.jsx   

        >PlanCCC 
        >>ComponentA.jsx      
        >>ComponentB.jsx      
   03. fun 
    ```
        001：function
        002：()=> 
    ```
2. style
    ``` 
        001：react-native-css
        002：StyleSheet.create
        003：内联式 嵌入式 外联式
    ```
3. 常量定义
    ```
        001：var 
        002：let 
        003：const
    ```
4. 代码格式 `eslint+prettier+editorconfig`
5. 其他

## 异常日志

---
`待定`

## 单元测试

---
`待定`