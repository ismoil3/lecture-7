![](https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcRk2uA11dVJwMCSXU_D8QOAxIIdPbmEpv498A&s)


![](https://i.ytimg.com/vi/CnozSz4wbBQ/maxresdefault.jpg)

**A JavaScript date is fundamentally specified as the time in milliseconds that has
elapsed since the epoch, which is defined as the midnight at the beginning of January
1, 1970, UTC (equivalent to the UNIX epoch). This timestamp is timezone-agnostic and
uniquely defines an instant in history**


*The Date() constructor creates Date objects. When called as a function, it returns a string
representing the current time.*



## *Creating Date Objects:*
new Date();

new Date(milliseconds)

new Date (date string)

new Date(year, month, day, hours,minutes,seconds,milliseconds)


``` js
const now = new Date();
console.log(now)
```


new Date( ) , string

``` js
const specificDate = new Date("2024-08-01");
console.log(specificDate);

```

new Date (milisecond)

```js
const dateFromMilliseconds = new Date(1627843200000);
console.log(dateFromMilliseconds);
```


new Date(year, month, day, hours,minutes ...)

```js
const customDate = new Date(2024, 7, 1, 12, 30, 0, 0);
console.log(customDate);
```





![](https://www.hubspot.com/hs-fs/hubfs/javascriptdate_3.webp?width=600&height=450&name=javascriptdate_3.webp)


getFullyar( )

Возвращает год в виде четырехзначного числа.

```js
const date = new Date();
console.log(date.getFullYear()); // Например, 2024

```

getMonth( )


Возвращает месяц (0-11). Январь - 0, Февраль - 1 и т.д.
```js
console.log(date.getMonth()); // Например, 7 для августа

```

getDate( )

Возвращает день месяца (1-31).
```js
console.log(date.getDate()); // Например, 1
```

getDay( )

 Возвращает день недели (0-6). Воскресенье - 0, Понедельник - 1 и т.д.
```js
console.log(date.getDay()); // Например, 4 для четверга
```

getHours( )

Возвращает часы (0-23).
```js
console.log(date.getHours()); // Например, 12
```

getMinuts( )

Возвращает минуты (0-59).


```js
console.log(date.getMinutes()); // Например, 30
```

getSeconds( )

 Возвращает секунды (0-59).
```js
console.log(date.getSeconds()); // Например, 45
```

getMilliseconds( )

 Возвращает миллисекунды (0-999).
```js
console.log(date.getMilliseconds()); // Например, 123
```

getTime( )

Возвращает количество миллисекунд, прошедших с 1 января 1970 года.
```js
console.log(date.getTime()); // Например, 1627843200000
```


![](https://cdn.goconqr.com/uploads/media/image/17500326/desktop_a4a1c94e-a3d1-4bd2-a1ba-3fbea8fdc15f.png)


setFullyar( )


Устанавливает год (и, опционально, месяц и день).
```js
const date = new Date();
date.setFullYear(2025, 7, 1); // Устанавливает 1 августа 2025 года
console.log(date);
```

setMonth( )

Устанавливает месяц (0-11) и, опционально, день.
```js
date.setMonth(11, 25); // Устанавливает 25 декабря текущего года
console.log(date);
```

setDate( )

Устанавливает день месяца (1-31).

```js
date.setDate(15); // Устанавливает 15-е число текущего месяца
console.log(date);
```


setHours( )

Устанавливает часы (0-23) и, опционально, минуты, секунды и миллисекунды.

```js
date.setHours(14, 30, 0, 0); // Устанавливает 14:30:00.000
console.log(date);
```


setMinutes(minutes, seconds, milliseconds): 

Устанавливает минуты (0-59) и, опционально, секунды и миллисекунды.

```js
date.setMinutes(45, 0, 0); // Устанавливает 45 минут
console.log(date);
```

setSeconds(seconds, milliseconds): 

Устанавливает секунды (0-59) и, опционально, миллисекунды.
```js
date.setSeconds(30, 0); // Устанавливает 30 секунд
console.log(date);

```

setMilliseconds(milliseconds):

 Устанавливает миллисекунды (0-999)

```js
date.setMilliseconds(500); // Устанавливает 500 миллисекунд
console.log(date);

```



setTime(milliseconds):

 Устанавливает время в миллисекундах с 1 января 1970 года.

 ```js
 date.setTime(1627843200000); // Устанавливает дату по количеству миллисекунд
console.log(date);
```