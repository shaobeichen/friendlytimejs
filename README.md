# friendlytime.js

> 友好时间的插件，将一个时间字符串格式（如2018-05-31 11:30:00）显示友好时间（如，1分钟内，2分钟前等等）。

## 快速开始
### 安装

```console
npm i friendlytimejs --save
```

### 使用
```js
import friendlytimejs from "friendlytimejs";
/**
 * @param str 指定的时间字符串，如yyyy-MM-dd HH:mm:ss
 * @param now 当前时间，允许时间戳，GMT时间。
 */
friendlytimejs.FriendlyTime('2018-06-04 13:20:00','2018-06-04 13:25:00');
```
推荐搭配使用[day.js](https://github.com/iamkun/dayjs)。如果你使用了day.js，那么过程即为
- 安装
```console
npm i friendlytimejs --save
npm i dayjs --save
```
- 使用
```js
import dayjs from "dayjs";
import friendlytimejs from "friendlytimejs";
/**
 * @param str 指定的时间字符串，如yyyy-MM-dd HH:mm:ss
 * @param now 当前时间，允许时间戳，GMT时间。
 */
friendlytimejs.FriendlyTime('2018-06-04 13:20:00',dayjs());
```