# The Past, Present, and Future of Local Storage for Web Applications

- For native applications, the operating system typically provides an abstraction layer for storing and retrieving 
  application-specific data like preferences or runtime state. These values may be stored in the registry, INI files,
  XML files, or some other place according to platform convention.

- Historically, web applications have had none of these luxuries. Cookies were invented early in the web’s history, 
  and indeed they can be used for persistent local storage of small amounts of data.

- HTML5 Storage is based on named key/value pairs. You store data based on a named key, then you can retrieve that data
 with the same key. The named key is a string. The data can be any type supported by JavaScript, including strings, 
 Booleans, integers, or floats. However, the data is actually stored as a string. If you are storing and retrieving 
 anything other than strings, you will need to use functions like parseInt() or parseFloat() to coerce your retrieved 
 data into the expected JavaScript datatype.

- If you want to keep track programmatically of when the storage area changes, you can trap the storage event.
 The storage event is fired on the window object whenever setItem(), removeItem(), or clear() is called and actually 
 changes something. For example, if you set an item to its existing value or call clear() when there are no named keys,
 the storage event will not fire, because nothing actually changed in the storage area.

- The storage event is supported everywhere the localStorage object is supported, which includes Internet Explorer 8.
 IE 8 does not support the W3C standard addEventListener (although that will finally be added in IE 9). Therefore,
 to hook the storage event, you’ll need to check which event mechanism the browser supports. (If you’ve done this before
 with other events, you can skip to the end of this section. Trapping the storage event works the same as every other event 
 you’ve ever trapped. If you prefer to use jQuery or some other JavaScript library to register your event handlers, 
 you can do that with the storage event, too.)

- While the past is littered with hacks and workarounds, the present condition of HTML5 Storage is surprisingly rosy.
 A new API has been standardized and implemented across all major browsers, platforms, and devices. As a web developer, 
 that’s just not something you see every day, is it? But there is more to life than “5 megabytes of named key/value pairs,” 
 and the future of persistent local storage is… how shall I put it… well, there are competing visions.One vision is an 
 acronym that you probably know already: SQL. In 2007, Google launched Gears, an open source cross-browser plugin which 
 included an embedded database based on SQLite. This early prototype later influenced the creation of the Web SQL Database
 specification. Web SQL Database (formerly known as “WebDB”) provides a thin wrapper around a SQL database, 
 allowing you to do things like this from JavaScript.