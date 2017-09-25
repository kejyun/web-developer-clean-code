# 變數


## 變數名稱必須要有意義

*錯誤示範：*

```javascript
// 年份
for(var i = 2000; i <= 2018, i++) {

}
```

**正確示範：**

```javascript
// 年份
for(var year = 2000; year <= 2018, year++) {

}
```

## 一般變數須用小寫及底線，用底線隔開有意義的文字

*錯誤示範：*

```javascript
// 字串
var userName = 'KJ';

// 整數
var AGE = 18;
```

**正確示範：**

```javascript
// 字串
var user_name = 'KJ';

// 整數
var age = 18;
```

## 陣列後方加入 `list` 特殊字，表示為陣列清單資料

*錯誤示範：*

```javascript
// 陣列
var Interest = [
    'Basketball',
    'Long board',
    'Cooking',
];
```

**正確示範：**

```javascript
// 陣列
var interest_list = [
    'Basketball',
    'Long board',
    'Cooking',
];
```

## 布林值前方加入 `is` 特殊字，表示為布林資料

*錯誤示範：*

```javascript
// 布林值
var EmailVerify = true;
```

**正確示範：**

```javascript
// 布林值
var is_email_verify = true;
```

## 物件或函式使用大駝峰式命名法（upper camel case），表示有可以呼叫的方法

*錯誤示範：*

```javascript
// 使用者物件
var user = {
    name: 'KJ'.
}

// 使用者物件資料集
var userCollections = [
    {
        name : 'KJ'
    },
    {
        name : 'KeJyun'
    }
];
```

**正確示範：**

```javascript
// 使用者物件
var User = {
    name: 'KJ'.
}

// 使用者物件資料集
var UserCollections = [
    {
        name : 'KJ'
    },
    {
        name : 'KeJyun'
    }
];
```


## 使用有意義且可以被搜尋的名稱

*錯誤示範：*

```javascript
// 設定使用者狀態
var User = {
    status : 'A',
};

User.status = 'I';
```

**正確示範：**

```javascript
// 定義類別整理常數
var UserConstant =  {
    STATUS_ACTIVE : 'A',
    STATUS_INACTIVE : 'I'
};

// 設定使用者狀態
var User = {
    status : UserConstant.STATUS_ACTIVE,
};

User.status = UserConstant.STATUS_INACTIVE;
```


## jQuery 物件名稱前面加上 $

*錯誤示範：*

```javascript
// 使用者群組區塊
var UserGroup = $('#user-group');
```

**正確示範：**


```javascript
// 使用者群組區塊
var $UserGroup = $('#user-group');
```
