# นี้มันปี 2016 แล้ว มาเรียนรู้ JavaScript ยุคสมัยใหม่กันเถอะ! 

![cover](images/Introduction3.png)

## สารบัญ

* [บทที่ 1 แนะนำภาษาจาวาสคริปต์](#บทที่-1-แนะนำภาษาจาวาสคริปต์)
* [บทที่ 2 ทวน ES5 (มาตรฐานเก่า)](#บทที่-2-ทวน-es5-มาตรฐานเก่า)
* [บทที่ 3 แนะนำ ES6](#บทที่-3-แนะนำ-es6)
* [บทที่ 4 แนะนำ ES7](#บทที่-4-แนะนำ-es7)
* [บทที่ 5 แนะนำ ES8](#บทที่-5-แนะนำ-es8)

## บทที่ 1 แนะนำภาษาจาวาสคริปต์

### เกริ่นนำ

* ภาษาจาวาสคริปต์ (JavaScript) เป็นภาษาโปรแกรมเชิงวัตถุแบบไดนามิกไทป์ (Dynamic types) ซึ่งไวยากรณ์ของมันได้นำโครงสร้างมาจากภาษายอดนิยมอย่างจาวา (Java) กับภาษาซี (C) 

* โปรแกรมที่เขียนขึ้นด้วยจาวาสคริปต์ จะต้องทำงานอยู่บนจาวาสคริปต์เอ็นจิ้น (JavaScript engine) ที่เป็นทั้งตัวแปลภาษา (Interpreter) และใช้รันโปรแกรม สำหรับการทำงานของจาวาสคริปต์ที่เราคุ้นเคยกันดี จะทำงานอยู่บนเว็บเบราเซอร์ เช่น Google Chrome, Firefox และ Internet Explorer เป็นต้น ซึ่งจะมีจาวาสคริปต์เอ็นจิ้นติดตั้งมาให้อยู่แล้ว

![จาวาสคริปต์ง่าย](images/chap01/EasyJavaScript.png)

* นักพัฒนาซอฟต์แวร์ส่วนใหญ่ล้วนรู้จักภาษาจาวาสคริปต์ ซึ่งถือว่านิยมใช้กันมากภาษาหนึ่งในโลก ถ้าศึกษาอย่างผิวเผินก็อาจคิดว่าง๊ายง่าย แต่เมื่อศึกษาลงลึก ๆ แล้ว จะพบว่ามัน**โคตรจะอินดี้ เป็นภาษาปราบเซียนตัวหนึ่ง** จนคนไม่ค่อยเข้าใจกันมากเท่าไรนัก จนหารู้ไม่ว่ามันมีความสามารถแฝงที่ซ้อนเร้นอยู่เยอะเลย

* จาวาสคริปต์ไม่ใช่ภาษา Java นะครับ คนละภาษา (คนมักสับสนกัน) 

![คำคมจาวา](images/chap01/quotes.png)

* คนส่วนใหญ่รู้แค่ว่าใช้จาวาสคริปต์ร่วมกับภาษา HTML (ปัจจุบันเวอร์ชั่น HTML5) กับ CSS (ปัจจุบันเวอร์ชั่น CSS3) เพื่อทำให้เว็บมันไดนามิก ฟุ้งฟิ้ง กรุ้งกิ๊ง (มันดังในฝั่ง Font-end มานาน)

* แต่ปัจจุบันนี้จาวาสคริปต์สมัยใหม่ มันก้าวหน้าไปไกลมาก ๆๆๆ เพราะสามารถทำงานอยู่ฝั่งเซิร์ฟเวอร์ได้ (Back-end) ด้วย Node.js แม้แต่เอาไปทำแอพบนโมบาย หรือแม้แต่โรบอท ก็ยังทำได้ด้วย ….อายย่ะ

![สถาปัตยกรรมเว็บ](images/chap01/webArchitectureEdit.PNG)

* องค์กร Ecma International (องค์กรจัดการมาตรฐานแห่งยุโรป) เป็นผู้กำหนดมาตรฐานจาวาสคริปต์ ซึ่งจะเรียกมาตรฐานนี้ว่า “ECMA-262” ส่วนตัวภาษาจาวาสคริปต์นั้น ก็จะมีชื่อเรียกเต็มยศอย่างเป็นทางการว่า “ภาษา ECMAScript“

![JavaScrit ECMAScript](images/chap01/JavaScriptECMAScript.jpg)

* ES6 (ECMAScript 2015) เป็นมาตรฐานใหม่ล่าสุดของจาวาสคริปต์ ประกาศออกมาเมื่อกลางเดือนมิถุนายนปี 2558 ซึ่งถือว่าเปลี่ยนแปลงเวอร์ชั่นครั้งใหญ่สุดในประวัติศาสตร์ของภาษานี้ หลังจากไม่ได้เปลี่ยนมาเกือบ 6 ปี (เวอร์ชั่นเก่าคือ ES5)

![ES5_ES6](images/chap01/ES5_ES6.PNG)

* ปีค.ศ. 2016 เวอร์ชั่นใหม่ ES7 (ECMAScript 2016) ก็ออกมาแหละ ส่วนปีหน้า 2017 ก็จะเป็นคิวของเวอร์ชั่น ES8 (ECMAScript 2017) จะออกมาเช่นกัน 

* ต้องเข้าใจอย่างนี้นะครัช เนื่อง ES6 มันใหญ่โตอลังการงานสร้างมาก คืนรอปล่อยออกมาหมดทีเดียว ก็คงรอหลายชาติภพ อาจทำให้มีเสียงบ่นตามมาได้ ด้วยเหตุนี้เข้าถึงเพิ่มฟีเจอร์เล็กยิบ ๆ ย่อย ๆ มาใส่ไว้ในเวอร์ชั่นหลัง ๆ แทน 

* โดยคาดว่าจากนี้ไป จะมีการประกาศเวอร์ชั่นใหม่ทุก ๆ ปี โดยให้คิดเสียว่า ES6 เหมือนโปรแกรมหลัก ส่วนเวอร์ชั่นที่ออกตามทีหลัง ไม่ได้ว่าจะเป็น ES7, ES8 และ ESXXXXX มันก็คือการอัพเดตซอฟต์แวร์ อะไรประมาณนี้

![ES7_ES8](images/chap01/ES7_ES8.PNG)

* API ที่ใช้ติดต่อกับ DOM หรือใช้งานร่วมกับ HTML5, CSS3 ใน ES6 เขาไม่ได้เปลี่ยนแปลงอะไรเลย

* ES6, ES7, ES8 มันเป็นแค่มาตรฐานใหม่สด ๆ ซิง ๆ ดังนั้นการใช้งานโดยตรงบนเว็บบราวเซอร์ (ปัจจุบันที่ผมเขียนอยู่นี้) ก็ยังไม่ support ทุกฟีเจอร์ ต้องมีตัวคอมไพล์ช่วยก่อน (ยังมีข้อจำกัดบางประการ) …แต่ถ้าใครใช้ Node.js เวอร์ชั่น 7 ขึ้นไป ก็จะรองรับ ES6 ได้ 98% (ES7 รองรับได้บางส่วน)

![ES5_ES6_ES7_ES8](images/chap01/Table_ES_version.PNG)

* TypeScript เป็นภาษาดัดแปลงมาจากจาวาสคริปต์ โดยทั้งนี้ไวยากรณ์และฟีเจอร์ต่างๆ จะมากกว่า อาจมองว่าเป็นซุปเปอร์เซตของจาวาสคริปต์อีกที (แน่นอนมันครอบคลุม ES6) ซึ่งเจ้าของภาษาคือ Microsoft

![TypeScript](images/chap01/TypeScript.PNG)

### ลองมาดูความนิยมของ ES6 กัน

![javascript_flavors](images/chap01/Javascript_flavors.PNG)

จากรูปเป็นผลสำรวจปี 2016 จะเห็นว่ามาตรฐานใหม่ ES6 คนเริ่มใช้งานเยอะ ไล่จี้จาวาสคริปต์แบบเก่าติดๆ แล้ว (ES5)

(ที่มา http://stateofjs.com/2016/flavors/)

### เครื่องมือในการพัฒนาจาวาสคริปต์ (IDE)

* มีให้ใช้ฟรีหลายตัวมาก เช่น Visual Studio Code, Sublime Text, Atom, Free JavaScript Editor, Aptana Studio, NetBeans, Eclipse ฯลฯ 
* หรือแม้แต่ใช้อิดิเตอร์ (Editor) ธรรมดา เช่น Notepad, Notepad++ และ EditPlus เป็นต้น 
* หรือถ้าเป็น geek หน่อย ก็จะใช้ Text Editor อย่าง Vim, Emacs เป็นต้น

![TypeScript](images/chap01/Quotes.png)

### Node.js มันคืออะไรตับไตใส้พุง?

ถ้าใครจับจาวาสคริปต์ยุคนี้ จะหนีไม่พ้นต้องรู้จัก Node.js …เอ๊ะ ว่าแต่มันคืออะไรล่ะ?

ถ้าอธิบายสั้นๆ มันคือตัวรันไทม์ (Runtime) ของภาษาจาวาสคริปต์ โดยที่เราไม่ต้องพึ่งพาเว็บบราวเซอร์เลย 

ด้วยเหตุนี้จึงสามารถรันจาวาสคริปต์นอกเว็บเบราเซอร์ได้ ซึ่งปัจจุบันเขานิยมนำ Node.js มาใช้งานฝั่งเซิร์ฟเวอร์ (Back-end) หรือจะทำงานตามลำพังเป็นแบบ Standalone ก็ย่อมได้นะลูกพี่

ถ้าสนใจเนื้อหาของ Node.js มากกว่านี้ ก็สามารถอ่าน ebook ที่ผมแจกฟรีได้ที่

* [วิธีติดตั้ง Node.js และ npm เบื้องต้น (Node.js เวอร์ชั่น 6)](http://ebooks.in.th/ebook/37385/วิธีติดตั้ง_Node.js_และ_npm_เบื้องต้น/)
* [Node.js เล่ม 1](http://www.ebooks.in.th/ebook/37714/เสียดายไม่ได้อ่าน_จาวาสคริปต์ฝั่งเซิร์ฟเวอร์_Node.js_(ฉบับย่อ)/)
* [Node.js เล่ม  2] (http://www.ebooks.in.th/ebook/37836/เสียดายไม่ได้อ่าน_จาวาสคริปต์ฝั่งเซิร์ฟเวอร์_Node.js_ฉบับย่อ_เล่ม2)
* [การใช้งาน MongoDB เบื้องต้น (แถมให้อีกอัน)](http://www.ebooks.in.th/ebook/37861/การใช้งาน_MongoDB_เบื้องต้น/)

*** ต้องสมัครเป็นสมาชิกของ http://www.ebooks.in.th ถึงจะโหลด PDF ได้

![my ebook](images/chap01/my_book.PNG)

ถ้าใครขี้เกียจสมัครเป็นสมัครชิก ก็ให้ใช้ลิงค์ดังต่อไปนี้แทน

* http://www.ebooks.in.th/ebook/37385/วิธีติดตั้ง_Node.js_และ_npm_เบื้องต้น/
* http://www.ebooks.in.th/ebook/37714/เสียดายไม่ได้อ่าน_จาวาสคริปต์ฝั่งเซิร์ฟเวอร์_Node.js_(ฉบับย่อ)/
* http://www.ebooks.in.th/ebook/37836/เสียดายไม่ได้อ่าน_จาวาสคริปต์ฝั่งเซิร์ฟเวอร์_Node.js_ฉบับย่อ_เล่ม2/
* http://www.ebooks.in.th/ebook/37861/การใช้งาน_MongoDB_เบื้องต้น/
* เล่มอื่นเผื่อใครสนใจ http://www.ebooks.in.th/adminho/

![read books](images/read_book.png)

###  ตัวอย่างจาวาสคริปต์บนเว็บเบราเซอร์ 

ตัวอย่างต่อไปนี้จะแสดงการเขียนจาวาสคริปต์ตามมาตรฐานเก่า ES5 ซึ่งจะต้องแทรกอยู่ภายใต้แท็ก < script > ...< /script > ของไฟล์ HTML โดยทั้งนี้จะสมมติว่าบันทึกเป็นไฟล์ index.html

*** ผมขอติ้งต่างว่า คุณเขียนจาวาสคริปต์บน HTML เป็นกันอยู่แล้วเนอะ

```js
<!-- ไฟล์ชื่อ index.html-->
<!DOCTYPE html>
<html>
<head></head>
<body>
	<h1 id="element1"></h1>
	<script>		
		// ซอร์สโค้ดตามมาตราฐานเก่า ES5   
		function say(message){
	    		var element = document.querySelector('#element1');
	    		element.innerHTML = message;			
		}
		say("Hello, world!");
</script>
</body>
</html>
```

โครงสร้างโปรเจค

```js
C:\ES6>
    |-- index.html
```

เมื่อดับเบิลคลิกที่ไฟล์ index.html จะปรากฏตามรูป

![Hello world](images/chap01/Hello_world_Edit.png)

### ตัวอย่างจาวาสคริปต์นอกเว็บเบราเซอร์

ต่อไปจะแสดงการใช้งานจาวาสคริปต์นอกเว็บเบราเซอร์ ด้วยการใช้ Node.js รันไฟล์จาวาสคริปต์ในฝั่งเซิร์ฟเวอร์

```js
var http = require('http');

http.createServer(function (request, response) {
  response.writeHead(200, {'Content-Type': 'text/plain'});
  response.end("Hello, world!");
}).listen(8001, '127.0.0.1');

console.log('Server running at http://127.0.0.1:8001/');
```

ซอร์สโค้ดข้างบน อย่าเพิ่งสนใจรายละเอียดนะครับ (มันนอกประเด็น) แต่จะสมว่าบันทึกเป็นไฟล์ server.js ดังโครงสร้างโปรเจคต่อไปนี้

```js
C:\ES6>
    |-- server.js
```

รันไฟล์ server.js ผ่านทาง Node.js ด้วยความสั่งต่อไปนี้  ตามรูป

![run node.js server.js](images/chap01/run_node.PNG)

*** อ่านวิธีติดตั้ง และใช้งาน Node.js เพิ่มเติม ได้จากหนังสือที่ผมแจกฟรีข้างต้นนะครับ

เมื่อเปิดเว็บเบราเซอร์แล้วกรอก URL เป็น http://127.0.0.1:8001/ ก็จะเห็นข้อความ Hello, world! แสดงออกมาทางหน้าเว็บเพจ ตามรูป

![result node.js server.js](images/chap01/Architecture_Node_Edit.js.PNG)

### ตัวอย่างการเขียน ES6 กับ ES7 บนเว็บเบราเซอร์

เนื่องจากเว็บเบราเซอร์ส่วนใหญ่จะใช้งานได้กับ ES5 ด้วยเหตุนี้จึงต้องนำซอร์สโค้ดที่เขียนด้วย ES6 มาคอมไพล์ ด้วยคอมไพเลอร์ที่เรียกว่า “transpiler” เพื่อแปลงจาก ES6 ให้กลายมาเป็นเวอร์ชั่น ES5 ที่เว็บเบราเซอร์ส่วนใหญ่ใช้งานได้ไปก่อน

#### Traceur

โดยตัวอย่างต่อไปนี้จะแสดงการเขียนจาวาสคริปต์บนเว็บเบราเซอร์ โดยใช้ Traceur ทำตัวเป็น transpiler (อย่าเพิ่งสนใจรายละเอียดซอร์สโค้ดที่ยกมาให้ดูนะครับ)

```js
<!-- ไฟล์ index.html-->
<!DOCTYPE html>
<html>
<head>

<!--  Traceur (ใช้เป็นตัว transpiler)-->
<script src="https://google.github.io/traceur-compiler/bin/traceur.js"></script>
<script src="https://google.github.io/traceur-compiler/bin/BrowserSystem.js"></script>
<script src="https://google.github.io/traceur-compiler/src/bootstrap.js"></script>

</head>
<body>
<h1 id="element1"></h1>
<script type="module">						// ต้องเขียนกำกับ type = "module"
	class Chat{								// class ไวยากรณ์ใหม่ของ ES6
		constructor(message) {				// constructor ไวยากรณ์ใหม่ของ ES6
			this.message = message;
		}
		say(){
			let element = document.querySelector('#element1');
			element.innerHTML = this.message;				
		}
	}		
	let chat = new Chat("Hello, world!");	// let ไวยากรณ์ใหม่ของ ES6
	chat.say();

	// ตัวอย่างโค้ด ES7 ชุดนี้ยังรันได้เฉพาะบน Google Chrome
	let array = ["A", "B", "C"];			// let ไวยากรณ์ใหม่ของ ES6
	console.log(array.includes("A"));   	// true    -- เมธอดของอาร์เรย์ที่เพิ่มเข้ามาใน ES7
</script>
</body>
</html>
```

จะสมมติว่าบันทึกเป็นไฟล์ index.html โดยมีโครงสร้างโปรเจคดังนี้

```js
C:\ES6>
    |-- index.html
```

เมื่อดับเบิลคลิกที่ไฟล์ index.html จะปรากฏตามรูป

![Hello world es6 es7](images/chap01/helloworld_es6_es7.png)


สังเกตในโค้ดจะต้องระบุ < script type="module" >

แต่ถ้าจะเขียนโค้ดจาวาสคริปต์ แยกออกมาเป็นไฟล์ .js เช่น mylib.js ก็สามารถทำได้ โดยจะมีโครงสร้างข้างล่าง

```js
C:\ES6>
    |-- index.html
    |-- mylib.js
```

ส่วนไฟล์ mylib.js ก็หน้าตาแบบนี้ไง แค่แยกโค้ดจาวาสคริปต์ออกมา

```js
class Chat{                             // class ไวยากรณ์ใหม่ของ ES6
    constructor(message) {              // constructor ไวยากรณ์ใหม่ของ ES6
        this.message = message;
    }
    say(){
        let element = document.querySelector('#element1');
        element.innerHTML = this.message;               
    }
}       

let chat = new Chat("Hello, world!");   // let ไวยากรณ์ใหม่ของ ES6
chat.say();

// ตัวอย่างโค้ด ES7 ชุดนี้ยังรันได้เฉพาะบน Google Chrome
let array = ["A", "B", "C"];            // let ไวยากรณ์ใหม่ของ ES6
console.log(array.includes("A"));       // true    -- เมธอดของอาร์เรย์ที่เพิ่มเข้ามาใน ES7
```

สามารถเขียนอ้างไฟล์ .js ได้ง่ายๆ ดังนี้

```js
<!-- ไฟล์ index.html-->
<!DOCTYPE html>
<html>
<head>

<!--  Traceur (ใช้เป็นตัว transpiler)-->
<script src="https://google.github.io/traceur-compiler/bin/traceur.js"></script>
<script src="https://google.github.io/traceur-compiler/bin/BrowserSystem.js"></script>
<script src="https://google.github.io/traceur-compiler/src/bootstrap.js"></script>

</head>
<body>
<h1 id="element1"></h1>

<script type="module">
import "./mylib.js";  	// อ้างไฟล์ .js
</script>

</body>
</html>
```

**หมายเหต** วิธีอิมพอร์ตไฟล์ด้วยวิธีนี้ ถ้าไปเปิดดูบน Google Chrome อาจไม่ทำงาน แต่ไม่ต้องซีเรียส เรามีทางแก้ไข แนะนำให้ไปอ่านหัวข้อ [Cross-origin resource sharing (CORS)] (#cross-origin-resource-sharing-cors)

#### Babel

ต่อไปจะแสดงการเขียนจาวาสคริปต์บนเว็บเบราเซอร์ โดยใช้ Babel ทำตัวเป็น transpiler (ผลการทำงานจะเหมือนตัวอย่างตอนใช้ Traceur )

```js
<!-- ไฟล์ index.html-->
<!DOCTYPE html>
<html>
<head>

<!--  Babel (ใช้เป็นตัว transpiler)-->
<script src="https://cdnjs.cloudflare.com/ajax/libs/babel-standalone/6.14.0/babel.min.js"></script>

</head>
<body>
<h1 id="element1"></h1>
<script type="text/babel">					// ต้องเขียนกำกับ type = "text/babel"
	class Chat{								// class ไวยากรณ์ใหม่ของ ES6
		constructor(message) {				// constructor ไวยากรณ์ใหม่ของ ES6
			this.message = message;
		}
		say(){
			let element = document.querySelector('#element1');
			element.innerHTML = this.message;				
		}
	}		
	let chat = new Chat("Hello, world!");	// let ไวยากรณ์ใหม่ของ ES6
	chat.say();

	// ตัวอย่างโค้ด ES7 ชุดนี้ยังรันได้เฉพาะบน Google Chrome
	let array = ["A", "B", "C"];			// let ไวยากรณ์ใหม่ของ ES6
	console.log(array.includes("A"));   	// true    -- เมธอดของอาร์เรย์ที่เพิ่มเข้ามาใน ES7
</script>
</body>
</html>
```

จะสมมติว่าบันทึกเป็นไฟล์ index.html โดยมีโครงสร้างโปรเจคดังนี้

```js
C:\ES6>
    |-- index.html
```

เมื่อดับเบิลคลิกที่ไฟล์ index.html จะปรากฏตามรูป

![Hello world es6 es7](images/chap01/helloworld_es6_es7.png)

สังเกตในโค้ดจะต้องระบุ < script type="text/babel" > หรือเขียนเป็น < script type="text/jsx" > ก็ได้เหมือนกัน

แต่ถ้าจะเขียนโค้ดจาวาสคริปต์ แยกออกมาเป็นไฟล์ .js เช่น mylib.js ก็สามารถทำได้ โดยจะมีโครงสร้างข้างล่าง (ไฟล์ .js หน้าตาเหมือนตอนใช้ Traceur)

```js
C:\ES6>
    |-- index.html
    |-- mylib.js
```

สามารถเขียนอ้างไฟล์ .js ได้ง่ายๆ ดังนี้ (สังเกตโค้ดดีๆ วิธีอิมพอร์ตไฟล์ .js จะต่างกับ Traceur เล็กน้อย)

```js
<!-- ไฟล์ index.html-->
<!DOCTYPE html>
<html>
<head>

<!--  Babel (ใช้เป็นตัว transpiler)-->
<script src="https://cdnjs.cloudflare.com/ajax/libs/babel-standalone/6.14.0/babel.min.js"></script>

</head>
<body>
<h1 id="element1"></h1>
<script type="text/babel" src="mylib.js">	// อ้างไฟล์ .js
</script>
</body>
</html>
```

**หมายเหต** วิธีอิมพอร์ตไฟล์ด้วยวิธีนี้ ถ้าไปเปิดดูบน Google Chrome อาจไม่ทำงาน แต่ไม่ต้องซีเรียส เรามีทางแก้ไข แนะนำให้ไปอ่านหัวข้อ [Cross-origin resource sharing (CORS)] (#cross-origin-resource-sharing-cors)

### โหลดไฟล์ Traceur กับ Babel มาเก็บไว้ที่เครื่องแบบออฟไลน์

#### Traceur แบบออฟไลน์

จากตัวอย่างก่อนๆ เวลาเขียน ES6 กับ ES7 บนว็บบราวเซอร์ด้วย Traceur ผมต้องอ้างถึงไฟล์ traceur.js, BrowserSystem.js และ bootstrap.js แบบออนไลน์ แต่ถ้าจะโหลดไฟล์นี้ (ทั้งหมดที่เกี่ยวข้อง) มาเก็บไว้ที่เครื่องแบบออฟไลน์ ก็ให้ใช้คำสั่ง npm ข้างล่าง (วิธีติดตั้งและใช้งาน npm ก็ตามหนังสือข้างบนที่แจกให้อ่านฟรี)

```js
C:\ES6>npm install -save traceur 
```

จะเห็นไฟล์ถูกโหลดเข้ามาเก็บ ได้แก่ traceur.js กับ BrowserSystem.js 

```js
C:\ES6\node_modules\traceur\bin
			                 |-- BrowserSystem.js
			                 |-- traceur.js
```

ส่วนไฟล์ bootstrap.js ก็จะอยู่ที่

```js
C:\ES6\node_modules\traceur\src
					         |-- bootstrap.js
```

#### Babel แบบออฟไลน์

สำหรับ Babel ก็เช่นกัน สามารถโหลดไฟล์ babel.js หรือ babel.min.js มาใช้แบบออฟไลน์ (เลือกใช้ไฟล์ไหนก็ได้) ด้วยคำสั่ง npm ดังนี้ 

```js
C:\ES6>npm install --save babel-standalone
```

จะเห็นไฟล์ถูกโหลดมาเก็บตามนี้

```js
C:\ES6\node_modules\babel-standalone
			             |-- babel.js
			             |-- babel.min.js
```

หรือไปที่เว็บข้างล่างแล้วเลือกโหลดไฟล์ทั้งสองนี้ก็ได้

https://github.com/Daniel15/babel-standalone/releases

*** Traceur กับ Babelเท่าที่ผมลองใช้งานดู มันยังไม่นิ่งเท่าไร ถ้าจะนำมันไปใช้งานยังไง ก็ควรหมั่นอัพเดตจากทีมสร้างเขาอีกทีนะครับ ...ที่สำคัญวิธีใช้งานแต่ละเจ้า ก็ดันแตกต่างกันอีกแฮะ! จนหนังสือที่ผมเขียนไป ถ้าใครลองทำตาม แล้วใช้งาน ES6 ไม่ได้ เค้าขอโทษแล้วกันน๊า! ยังไงเดี่ยวขออัพเดตโค้ดล่าสุดที่เว็บนี้แล้วกันเนอะ

### วิธีคอมไพล์จาก ES6 ให้เป็น ES5 ด้วยมือตนเอง

#### Traceur

เราสามารถใช้กระบวนท่าแปลงซอร์สโค้ดจาก ES6 เป็น ES5 ด้วยมือตนเอง ด้วยการเปิดคอมมานไลน์ขึ้นมา (ตัวอย่างจะใช้วินโดวส์) แล้วเรียกสคริปต์ traceur ซึ่งถ้าคุณทำตามตัวอย่างก่อนหน้า ที่แนะวิธีโหลดไฟล์ Traceur มาเก็บแบบออฟไลน์ ด้วยคำสั่ง npm install -save traceur ก็ให้ไปที่โฟลเดอร์ ...\node_modules\ .bin จะเห็นไฟล์สคริปดังนี้

```js
C:\ES6\node_modules\.bin
			 		|-- traceur
			 		|-- traceur.cmd			 
```

จากไฟล์ mylib.js ในตัวอย่างก่อนหน้านี้ (โค้ด ES6) 

```js
C:\ES6>
    |-- index.html
    |-- mylib.js
```

เราก็สามารถเรียกสคริปต์ traceur ให้มาทำการคอมไฟล์ mylib.js เพื่อแปลงเป็น ES5 ได้คำสั่งดังนี้

```js
C:\ES6\node_modules\.bin>traceur --out ../../out/mylib.js --script ../../mylib.js
```
(ถ้าติดตั้ง Traceur ด้วยคำสั่ง npm install -g traceur ก็ไม่ต้อง cd มาที่ C:\ES6\node_modules\ .bin)

สำหรับไฟล์ที่ถูกแปลงเป็น ES5 จะเก็บอยู่ที่โฟลเดอร์ out\mylib.js

```js
C:\ES6>
    |-- index.html
    |-- mylib.js
    |-- out
    	 |-- mylib.js
```	

ถ้าแอบไปเปิดไฟล์ out\mylib.js ก็จะเห็นว่าโค้ดถูกแปลงเป็น ES5 หน้าตาเรียบร้อยดังนี้

```js
var Chat = function() {
  "use strict";
  function Chat(message) {
    this.message = message;
  }
  return ($traceurRuntime.createClass)(Chat, {say: function() {
      var element = document.querySelector('#element1');
      element.innerHTML = this.message;
    }}, {});
}();
var chat = new Chat("Hello, world!");
chat.say();
var array = ["A", "B", "C"];
console.log(array.includes("A"));
```

จากตัวอย่างเดิม ก็สามารถเขียนใหม่ได้ดังนี้

```js
<!-- ไฟล์ index.html-->
<!DOCTYPE html>
<html>
<head>

<!--  ระบุตัว transpiler -->
<script src="node_modules/traceur/bin/traceur-runtime.js"></script>

</head>

<body>
<h1 id="element1"></h1>

<!-- ไฟล์ .js ที่ถูกแปลงเป็น ES5 -->
<script src="out/mylib.js"></script>

</body>
</html>
```

ซึ่งผลการทำงานจะเหมือนกับตัวอย่างก่อนๆ ที่ยกมา

#### Babel

สำหรับ Babel ก็เช่นกัน สามารถใช้กระบวนท่าแปลงซอร์สโค้ดจาก ES6 ให้เป็น ES5 ด้วยมือตนเอง โดยทำตามตัวอย่างจากเว็บต้นทางผู้สร้าง เขาจะแนะนำตามนี้

```js
var input = 'const getMessage = () => "Hello World";';
var output = Babel.transform(input, { presets: ['es2015'] }).code;
```

จากตัวอย่างเดิม ก็สามารถเขียนใหม่ได้ดังนี้

```js
<!-- ไฟล์ index.html-->
<!DOCTYPE html>
<html>
<head>

<!--  ระบุตัว transpiler -->
<script src="https://cdnjs.cloudflare.com/ajax/libs/babel-standalone/6.14.0/babel.min.js"></script>

</head>
<body>
<h1 id="element1"></h1>
<script>                  // ไม่ต้องเขียนกำกับ type = "text/babel"
	
	// ใช้ Template Strings ของ ES6 เขียนโค้ดจาวาสคริปต์
	var input = `
	class Chat{                             // class ไวยากรณ์ใหม่ของ ES6
		constructor(message) {              // constructor ไวยากรณ์ใหม่ของ ES6
			this.message = message;
		}
		say(){
			let element = document.querySelector('#element1');
			element.innerHTML = this.message;               
		}
	}       

	let chat = new Chat("Hello, world!");   // let ไวยากรณ์ใหม่ของ ES6
	chat.say();

	// ตัวอย่างโค้ด ES7 ชุดนี้ยังรันได้เฉพาะบน Google Chrome
	let array = ["A", "B", "C"];            // let ไวยากรณ์ใหม่ของ ES6
	console.log(array.includes("A"));       // true    -- เมธอดของอาร์เรย์ที่เพิ่มเข้ามาใน ES7
	`;

	
	var output = Babel.transform(input, { presets: ['es2015'] }).code; // คอมไฟล์ ES6 เป็น ES5
	eval(output);	// ประมวลผล
</script>
</body>
</html>
```

ซึ่งผลการทำงานจะเหมือนกับตัวอย่างก่อนๆ ที่ยกมา

### Cross-origin resource sharing (CORS) 

โดยปกติแล้วเว็บเพจ จะไม่สามารถแชร์  resources ข้าม domain กันได้ (เช่น ฟอนต์, ไฟล์จาวาสคริปต์ และรูปภาพ เป็นต้น) เพราะมันเป็นเรื่องของความปลอภัย (same-origin policy)

คราวนี้ถ้าเขียนจาวาสคริปต์แบบแยกไฟล์ .js แล้วอิมพอร์ตเข้ามา (จากตัวอย่างก่อนหน้านี้ ผมอิมพอร์ตไฟล์ mylib.js เข้ามา ด้วยวิธี Traceur หรือ Babel) เมื่อนำไปเปิดบน Google Chrome อาจทำงานไม่ได้  (ซวยแล้วไง!)  เพราะเมื่อไปดูที่ console จะเห็นมันฟ้องเรื่อง Cross origin ดังรูป

![Hello world es6 es7](images/chap01/errorOnChome.png)

แต่เราสามารถหลีกเลี่ยงกฏข้อนี้ได้ โดยใช้ Cross-origin resource sharing (CORS) ซึ่งเป็นกลไกอนุญาตให้ resources บนเว็บเพจ ถูกเข้าถึงจาก Domain อื่นได้


**วิธีการแก้ปัญหา**

__วิธี1__

สามารถทำได้ง่ายๆ เพียงแค่บอกให้เว็บเซิร์ฟเวอร์ เพิ่มค่าต่อไปนี้ลงไปใน HTTP Header (วิธีกำหนดค่านี้ ต้องดูที่คู่มือของเซิร์ฟเวอร์แต่ละเจ้าเอาเอง)

```js 
Access-Control-Allow-Origin: *
```

จริงๆ ทำแบบนี้ก็ดูไม่ปลอดภัยเท่าไร ทางที่ดีควรให้สิทธิเฉพาะ url เท่าที่จำเป็น ตัวอย่างเช่น

```js
Access-Control-Allow-Origin: http://www.example.com http://test.example.com 
```

(ที่มา http://manit-tree.blogspot.com/2012/07/cross-origin-resource-sharing.html)


__วิธีที่ 2__

ถ้าเราไม่ได้เขียนเว็บ แล้วเทสบนเว็บเซิร์ฟเวอร์ อารมณ์ทดสอบเว็บบนเครื่องตัวเองแบบ local ก็ต้องเปิด Google chrome ด้วยท่าพิศดาร โดยปลดความปลอดภัยเรื่องนี้ออก เพื่อให้มันทำ CORS ได้

บนวินโดวส์ก็ให้ไปที่คอมมานไลน์  แล้วพิมพ์คำสั่งตามนี้ เมื่อนั้น Google Chrome ก็จะเปิดขึ้นมา แล้วถึงเปิดไฟล์ HTML ตามทีหลัง

```js 
chrome.exe --user-data-dir="C:/Chrome dev session" --disable-web-security
```

หรือจะระบุชื่อไฟล์ HTML ให้เปิดขึ้นมาพร้อมกับ Google Chrome ก็ได้
```js 
chrome.exe --user-data-dir="C:/Chrome dev session" --disable-web-security "c:\ES6\index.html"

```

อีกวิธีหนึ่งง่ายดี ให้ไปที่ Shortcut ของ Google Chrome แล้วคลิกขวาเปิดมันขึ้นมา จากนั้นจึงเพิ่มค่าต่อไปนี้ตรงช่อง "Target:" หลังข้อความเดิม

```js 
--user-data-dir="C:/Chrome dev session" --disable-web-security  
```

![Hello world es6 es7](images/chap01/howto_open_chrome_edit.png)

ต่อไปนี้ ก็ให้เปิดที่ Shortcut ของ Google Chrome ก่อนเสมอ แล้วหลังจากนั้น จึงเปิดไฟล์ HTML ตามทีหลัง


ส่วนบน OSX กับ Linux ผมไม่มีเครื่องลองครับ จึงไม่กล้าเขียน ลองดูเพิ่มเติมได้ที่ 

http://stackoverflow.com/questions/3102819/disable-same-origin-policy-in-chrome)


__วิธีที่ 3__

จากไฟล์ index.html ที่มีปัญหาเวลาเปิด Google Chrome แล้วไม่ทำงาน

```js
C:\ES6>
    |-- index.html
    |-- mylib.js
```

ให้ลองใช้เซิร์ฟเวอร์จำลอง จาก Node.js แต่ก่อนอื่นจะให้ติดตั้งเซิร์ฟเวอร์ที่ว่า ก็คือ live-server ด้วยคำสั่ง npm ดังนี้

```js
npm install -g live-server
```

จากนั้นก็ cd ไปที่ C:\ES6\ ต่อด้วยสั่งให้ live-server ทำการรัน index.html ด้วยคำสั่งง่ายๆ ดังนี้

```js
C:\ES6>live-server
```

เมื่อนั้นเว็บบราวเซอร์ที่ถูกตั้งไว้เป็นดีฟอลต์ ก็จะเด้งขึ้นมา และเปิดไฟล์ index.html อย่างอัตโนมัติ หรือถ้าเครื่องเรา Google Chrome ไม่ได้ตั้งเป็นดีฟอลต์ ก็ให้กรอก url ตรงๆ เป็น http://127.0.0.1:8080/ ตามรูป

![Hello world es6 es7](images/chap01/run_with_live-server.png)

** เสริมนิดหนึ่ง ถ้าใครใช้ Python ก็อาจใช้เซิร์ฟเวอร์จำลองได้ด้วยเช่นกัน อย่างกรณีผมใช้ Python 3 ก็จะพิมพ์คำสั่งดังนี้

```js
C:\ES6>python -m http.server 8080
```

จากนั้นก็เปิด Google Chrome ขึ้นมาโดยกรอก url เป็น http://127.0.0.1:8080/


### ตัวอย่างการเขียน ES6 กับ ES7 บน Node.js

ต่อไปจะแสดงการเขียนจาวาสคริปต์ด้วย ES6 กับ ES7 แล้วสั่งรันผ่านทาง Node.js โดยตรง ไม่ต้องใช้  transpiler (หรือจะใช้ ก็แล้วแต่ครับ)

*** ทั้งนี้ Node.js เวอร์ชั่น 7 ขึ้นไปก็จะรองรับ ES6 ได้ 98%

*** ส่วน ES7 ผมยังไม่ค่อยแน่ใจสักเท่าไร

```js
class Chat{                 			// class ไวยากรณ์ใหม่ของ ES6
    constructor(message) {      		// constructor ไวยากรณ์ใหม่ของ ES6
        this.message = message;
    }
    say(){
        console.log(this.message);
    }
}       

let chat = new Chat("Hello, world!");   // let ไวยากรณ์ใหม่ของ ES6
chat.say();                 			// "Hello, world!"

let array = ["A", "B", "C"];
console.log(array.includes("A"));   	// true    -- เมธอดของอาร์เรย์ที่เพิ่มมาใน ES7
```

จะสมมติว่าบันทึกเป็นไฟล์ test.js โดยมีโครงสร้างโปรเจคดังนี้

```js
C:\ES6>
    |-- test.js
```

รันไฟล์ test.js ผ่านทาง Node.js ด้วยความสั่งต่อไปนี้ ตามรูป

![node.js es6 es7](images/chap01/node.js_es6_es7.png)


## บทที่ 2 ทวน ES5 (มาตรฐานเก่า)

![cover](images/chap02/Introduction_edit1.png)

จาวาสคริปต์ยังคงความอินดี้ของมาตรฐานตัวเดิมเอาไว้เช่นเดิม (ES5) โดยไม่ได้ลบเลือนจางหายไปไหนเลย ซึ่งบทนี้เราจะมาทบทวนคร่าวๆ กัน

(บทนี้ ยังไม่เสร็จดีครับ)
### Comments

คอมเมนต์ในจาวาสคริปต์ ก็จะเหมือนภาษาที่มีรากฐานมาจากภาษา C โดยจะใช้เครื่องหมาย // นำหน้าประโยคที่ต้องการคอมเมนต์ได้เพียงบรรทัดเดียวเท่านั้น 

```js
var x = 10; 	//This is an example.
```
แต่ถ้าต้องการคอมเมนต์หลายๆ บรรทัด ก็ให้ใช้เครื่องหมาย /*… */ มาครอบเปิดและปิดท้าย กลุ่มประโยคที่ต้องการ 

```js
/* This is an example
ECMAScript 6 is very easy*/
```
### console.log

ประโยคคำสั่ง console.log() จะเป็นฟังก์ชั่น (Function) ในจาวาสคริปต์ ที่ใช้ประโยชน์ในแง่ของการดีบั๊ก (Debug) เพื่อแสดงข้อความออกทางหน้าคอนโซล (Console) 

```js
<!DOCTYPE html>
<html>
<head></head>

<body>
	<h1>Hello, world!</h1>
	<script>		
             console.log("Hello, world!");
	</script>
</body>
</html>
```

จะปรากฏผลลัพธ์ดังนี้

![Hello world](images/chap02/hello_word_console.png)

### Semicolon

จาวาสคริปต์ถือว่าเป็นภาษาหนึ่ง ที่ไม่ต้องใช้เครื่องหมายเซมิโคลอน (;) ต่อท้ายแต่ละประโยคคำสั่งก็ได้ ดังตัวอย่าง

```js
// ไม่ต้องมี ; ต่อท้ายประโยคก็ได้
console.log("Hello world")

// หรือมี ; ต่อท้ายประโยคก็ได้
console.log("Hello world");
```

แต่ถ้ามี 2 ประโยคคำสั่งขึ้นไป เขียนติดกันอยู่ภายในบรรทัดเดียวกัน จะต้องมี ; แบ่งคันเอาไว้เสมอ

```js
// แบบนี้จะเกิด Syntax Error เพราะไม่มี ; แบ่งคั่นประโยค
// console.log("Hello, world!")  console.log("Hello, world!");

console.log("Hello, world!") ; console.log("Hello, world!")
// Hello, world!
// Hello, world!
```
แต่ทั้งนี้เขาจะนิยมใส่ ; ต่อท้ายประโยคเหมือนหลายๆ ภาษา

![semicolon](images/chap02/semicolonForgot2.png)

### การประกาศตัวแปร

การประกาศตัวแปร จะใช้คีย์เวิร์ด var นำหน้าชื่อตัวแปร ดังตัวอย่าง

```js
var  x = 100;	
```

หรือจะประกาศตัวแปรให้อยู่ในบรรทัดเดียวกันก็ได้ ดังตัวอย่าง
```js
var  x = 1, y = 2, z = 3;	// ประกาศตัวแปร x, y และ z ให้อยู่ในบรรทัดเดียวกัน
```

แต่ถ้าเราไม่ได้กำหนดค่าเริ่มต้นให้กับตัวแปร ตอนประกาศตัวแปร ก็จะมีค่าเป็น undefined ดังตัวอย่าง

```js
var x; 	    
console.log(x); 			// undefined
```
### Literals
สำหรับข้อมูล (Literals) ที่สามารถกำหนดค่าให้กับตัวแปรได้นั้น ในจาวาสคริปต์ก็จะมีหลากหลายชนิดข้อมูล แต่โดยหลัก ๆ จะมีอยู่ 2 แบบได้แก่ 

* ข้อมูลพื้นฐาน (Primitives data) 
* อ็อบเจ็กต์ (Object)

สำหรับข้อมูลพื้นฐาน จะแยกย่อยได้นี้

* null 
* undefined 
* ตัวเลข (Number) 
* สตริง (String) รวมทั้งเทมเพลตสตริง (Template String) 
* บูลีน (Boolean) 
* ซิมโบล (Symbol)

### Function

ตัวอย่างต่อไปนี้จะเป็นการประกาศฟังก์ชั่น

```js
function calculate(param1, param2){
	return param1 * param2;
}
```

ส่วนวิธีเรียกใช้งานฟังก์ชั่น ก็จะเหมือนกับภาษาเขียนโปรแกรมทั่ว ๆ ไป ดังตัวอย่าง

```js
var result = calculate(10, 2);	
console.log(result);		// 20
```

### Hoist

การประกาศฟังก์ชั่น รวมทั้งการประกาศตัวแปรแบบ var มันจะลอยขึ้นไปประกาศอยู่ข้างบนสุดของขอบเขตการมองเห็น ดังตัวอย่าง

```js
function myFunction(num){
	// สามารถมองเห็นตัวแปร value		
	console.log(value);			// undefined

	if(num > 10) {
		var value = num*10;		// ประกาศตัวแปร value ที่ตรงนี้ แต่มองเห็นได้ทั่วฟังก์ชั่น
		
		/* ซอร์สโค้ด */
		
	} else {
		
		// ถ้าเงื่อนไขประโยค if เป็นเท็จ ก็จะเข้ามาทำงานที่ else 
		// ซึ่งจะเห็นตัวแปร value มีค่าเป็น undefined	
	
		console.log(value);		// undefined
	}			
	
	// สามารถมองเห็นตัวแปร value ได้ หลังจากประโยค if …else ทำงานเสร็จสิ้น
	console.log(value);			
}
```

จากตัวอย่างซอร์โค้ดดังกล่าวที่ยกมาให้ดู จริง ๆ แล้ว จาวาสคริปต์จะทำการแปลงซอร์สโค้ดให้มีหน้าตาดังต่อไปนี้

```js
function myFunction(num){
	var value; 				// ประกาศตัวแปร value โดยไม่มีค่าเริ่มต้น จึงทำให้มีค่าเป็น undefined
	console.log(value);		// undefined
	
	if(num > 10) {
		value = num*10;		// บรรทัดนี้เป็นเพียงการกำหนดค่าให้กับตัวแปร value
		
		/* ซอร์สโค้ด */
		
	} else {
       
	   console.log(value);	// undefined
	   
	}	
	
	console.log(value);		
}
```

(บทนี้ ยังไม่เสร็จดีครับ)


## บทที่ 3 แนะนำ ES6

(บทนี้ ยังไม่เสร็จดีครับ)

### 3.1 การประกาศตัวแปร และการกำหนดค่า

#### การประกาศตัวแปรแบบ let

การประกาศตัวแปรแบบ var จะถูกลอยขึ้นไปประกาศอยู่ด้านบนสุด (hoist)

แต่การใช้ let ในการประกาศตัวแปร ขอบเขตการมองเห็นเริ่มตั้งแต่จุดที่ประกาศใช้งานภายในบล็อก (ไม่ลอยขึ้นไปอยู่บนสุด หรือ hoist) ส่วนตัวแปรก็จะมีชีวิตอยู่ภายในบล็อกปัจจุบัน  ดังตัวอย่าง

```js
function calculate(num){
	if (num > 10) {
		let value = num*10;		// ประกาศตัวแปรแบบ let 
		
		// ซอร์สโค้ดส่วนที่เหลือ
		console.log(value);		// มองเห็นตัวแปร value
	} else {
		
		// มองไม่เห็นตัวแปร value		
		
	}	
	
	// มองไม่เห็นตัวแปร value
}
```
#### ตัวแปรค่าคงที่

การประกาศตัวแปรค่าคงที่ (Constants) จะใช้คีย์เวิร์ด const นำหน้าชื่อตัวแปร 

แต่เราต้องกำหนดให้มันมีค่าเริ่มต้น ตั้งแต่ประกาศตัวแปรครั้งแรก และหลังจากนั้นก็ห้ามไปแก้ไขค่าอะไรภายหลังเด็ดขาด ดังตัวอย่าง

```js
const MAX_COUNT = 100;		// ประกาศถูกต้องตามไวยากรณ์
const MAX_VALUE;			// เกิด error เพราะไม่ได้กำหนดค่าตั้งต้นให้แต่แรก
const MESSAGE = "Hello";	// ประกาศถูกต้องตามไวยากรณ์
MESSAGE = "Bye"; 			// เกิด error เพราะไปแก้ไขตัวแปรค่าคงที่ภายหลังประกาศใช้งานแล้ว ซึ่งจะทำไม่ได้
```

(เดี่ยวมาเขียนต่อให้เสร็จ)

### 3.2 Functions

#### Arrow Functions

ในหลาย ๆ ภาษาจะมี "Lambda expressions" ซึ่งคนที่มาจากภาษาอื่นอาจรู้จักกันดีอยู่แล้ว เช่น 

* ใน C# จะใช้สัญลักษณ์ => 
* หรือถ้าเป็นจาวา (ตั้งแต่ Java 8) จะใช้สัญลักษณ์ -> 
* ใน Python ใช้คีย์เวิร์ด  lambda

แต่สำหรับจาวาสคริปต์จะเรียกว่า "Arrow Functions" แปลตรงตัวก็คือ "ฟังก์ชั่นลูกศร" โดยใช้เครื่องหมาย => (มันคือฟังก์ชั่นไร้ชื่อ ที่ไม่ได้ใช้คีย์เวิร์ด function) ซึ่งมันเขียนได้หลายวิธีมากๆ ดังตัวอย่างต่อไปนี้

##### ตัวอย่างที่ 1

```js
let arrowFunc = function(value){		
	return value;
};

console.log(arrowFunc(122)); 	// 122
```

จากตัวอย่างดังกล่าว สามารถเปลี่ยนมาเขียนแบบฟังก์ชั่นลูกศร ได้ดังนี้

```js
let arrowFunc = value => { 
	return value;
};

// เรียกใช้ฟังก์ชั่นได้เหมือนปกติธรรมดา
console.log(arrowFunc(122)); 	// 122
```
##### ตัวอย่างที่ 2

```js 
// เหมือนในตัวอย่างที่ 1 แต่การเขียนจะสั้นและกระชับกว่า
// ไม่ต้องมีเครื่องหมายปีกกา {....} ครอบบอดี้ฟังก์ชั่น รวมทั้งไม่ต้องเขียนประโยคคำสั่ง return
let arrowFunc = value => value;	
console.log(arrowFunc(122)); 	// 122
```

จะเสมือนเขียนเป็น

```js 
let arrowFunc = function(value){		
	return value;
};
console.log(arrowFunc(122)); 	// 122
```

อีกตัวอย่างหนึ่ง

```js
let arrowFunc2 = value => console.log(value);	
arrowFunc2(122); 				// 122
```

จะเสมือนเขียนเป็น

```js
let arrowFunc2 = function(value){		
	return console.log(value);
};
arrowFunc2(122); 				// 122
```

##### ตัวอย่างที่ 3

```js
// ฟังก์ชั่นลูกศรที่ไม่มีการประกาศพารามิเตอร์อะไรเลย
let arrowFunc = () => 122; 	
console.log(arrowFunc()); 		// 122
```

จะเสมือนเขียนเป็น

```js 
let arrowFunc = function(){
	return 122;
};
console.log(arrowFunc()); 		// 122
```

##### ตัวอย่างที่ 4

```js
// ฟังก์ชั่นลูกศรที่ไม่มีพารามิเตอร์ และตัวบอดี้ของฟังก์ชั่นก็ว่างเปล่า
let arrowFunc = () => {}; 
arrowFunc();
```

จะเสมือนเขียนเป็น

```js
var arrowFunc = function(){};
arrowFunc();
```

##### ตัวอย่างที่ 5

```js
// ใส่เครื่องหมายวงเล็บ เพื่อครอบอ็อบเจ็กต์ที่ถูกรีเทิร์นออกมา
let getFont = () => ( { color: "red", size: 200 } ); 
console.log(getFont());			// {color: "red", size: 200}
```

จะเสมือนเขียนเป็น

```js
let getFont = function(){
	return {color: "red", size: 200};
};
console.log(getFont());			// {color: "red", size: 200}
```

##### ตัวอย่างที่ 6

```js
// มีวงเล็บครอบพารามิเตอร์เอาไว้
let sum = (val1, val2, val3) => val1 + val2 + val3;
console.log(sum(1,2,3));		//  6
```

จะเสมือนเขียนเป็น

```js 
let sum = function(val1, val2, val3){
	return val1 + val2 +val3;
};
console.log(sum(1,2,3));		//  6
```

##### ตัวอย่างที่ 7

```js
// ฟังก์ชั่นลูกศรที่ใช้พารามิเตอร์แบบดีฟอลต์
let sum = (val1 = 1, val2 = 2, val3 = 3) => val1 + val2 + val3;
console.log(sum());				//  6
```

จะเสมือนเขียนเป็น

```js
let sum = function(val1 = 1, val2 = 2, val3 = 3){
	return val1 + val2 +val3;
};
console.log(sum());				//  6
```

##### ตัวอย่างที่ 8

```js
// ฟังก์ชั่นลูกศรที่ใช้พารามิเตอร์แบบเรสต์ 
let max = (...value) => Math.max(...value);
console.log(max(1, 2, 3, 6));	// 6
```

จะเสมือนเขียน

```js
let max = function(...value){	// พารามิเตอร์แบบเรสต์
	return Math.max(...value);	// โอเปอเรเตอร์สเปรด
};
console.log(max(1, 2, 3, 6));	// 6
```

(ยังเขียนไม่เสร็จดี)

### 3.3 Template strings

เทมเพลตสตริง (Template strings) จะใช้เครื่องหมาย back-tick (ตัวอักษร grave accent) มาครอบข้อความเอาไว้ (เครื่องหมายจะคล้ายๆ กับคำพูดเดี่ยว แต่มันจะเอนไปด้านหน้าเล็กน้อย) ดังตัวอย่าง

```js
let msg = `JavaScript`;

console.log(msg);             	// "JavaScript"
console.log(msg.length);      	// 10 
console.log(typeof msg);      	// "string"
```

#### เขียนสตริงหลายบรรทัด

เทมเพลตสตริงสามารถเขียนข้อความได้มากกว่า 1 บรรทัด (Multiline strings) ดังตัวอย่าง

```js
let div = `<div>
<h1>Hello world</h1>
</div>`;

console.log(div);
```

แสดงผลลัพธ์เป็น

```js
<div>
	<h1>Hello world</h1>
</div>
```
#### นิพจน์ในเทมเพลตสตริง

ปกติแล้วการเขียนนิพจน์ร่วมกับสตริงแบบเดิมจะดูยุ่งยากมาก เพราะต้องใช้เครื่องหมายบวก (+) เชื่อมสตริงกับนิพจน์ต่าง ๆ เข้าด้วยกัน ดังตัวอย่าง

```js
let a = 5, b = 10, c = 100;

console.log("Price $" + ((a*b).toFixed(2)) + ", not " + (c + a) );   // "Price $50.00, not 105"
```

แต่ถ้าลองเปลี่ยนมาใช้เทมเพลตสตริง ก็สามารถยัดนิพจน์เข้าไปอยู่ในสตริงได้เลย ดังตัวอย่าง

```js
let a = 5, b = 10, c = 100;

console.log(`Price $${(a*b).toFixed(2)}, not ${c + a}` );  		// "Price $50.00, not 105"
```

### 3.4 Symbols

(เดี่ยวมาเขียน)

### 3.5 Objects

(เดี่ยวมาเขียน)

### 3.6 คลาส

คลาสใน ES6 จะเหมือนกับภาษาโปรแกรมเชิงวัตถุอื่น ๆ (OOP: Object Oriented Programming) ที่เปรียบได้เป็นพิมพ์เขียวเอาไว้สร้างอ็อบเจ็กต์ โดยตัวอย่างต่อไปนี้จะแสดงการประกาศคลาส Car ขึ้้นมา (ยังไม่มีสมาชิกอะไรอยู่ข้างใน)

```js
class Car { 
	// สมาชิกภายในคลาส ยังไม่ได้ประกาศ 
}	
```

มันก็เหมือนๆ ภาษาอื่น  เราสามารถใช้โอเปอเรอตร์ new สร้างอ็อบเจ็กต์จากคลาส Car ข้างต้นขึ้นมาได้

```js
let car1 = new Car();
let car2 = new Car();
let car3 = new Car();
```

#### สมาชิกคลาส

ในคลาสสามารถมีสมาชิกดังต่อไปนี้

1) สมาชิกที่เป็นคอนสตรัคเตอร์ (constructor) โดยใช้เมธอดที่ชื่อ constructor ทำหน้าที่เป็นคอนสตรัคเตอร์เหมือนในภาษา OOP อื่นๆ

2) สมาชิกที่เป็นเมธอด

*** ทั้งนี้สมาชิกของคลาส ไม่ว่าจะเป็นคอนสตรัคเตอร์ และเมธอดต่างๆ ไม่ต้องใช้เครื่องหมายจุลภาค , แบ่งคั่นนะ

```js
class Car { 
    constructor(param){ 		// ประกาศคอนสตรัคเตอร์
		console.log(param);
    }
	
	drive(){					// ประกาศเมธอด
		console.log("The car is running");
	}
}

let carObj = new Car("red");	// "red"
carObj.drive();					// "The car is running"
```

มีข้อสังเกต ในภาษา C++, Java, C# สามารถประกาศตัวแปรเป็นสมาชิกประเภทหนึ่งในคลาสได้ 
แต่เสียใจด้วยใน ES6 ไม่สามารถประกาศตัวแปร เป็นสมาชิกในคลาสได้ ...เว้นแต่ใช้ภาษา TypeScript เราก็สามารถประกาศได้

ถึงกระนั้นก็ดีสามารถประกาศพร็อพเพอร์ตี้ที่เป็นตัวแปรขึ้นมาได้ ด้วยการใช้ this.xxx ภายในคอนสตรัคเตอร์ ดังตัวอย่าง
(ในเมธอดก็ประกาศได้ แต่อาจผิดหลักการ OOP ซึ่งคอนสตรัคเตอร์ ควรทำหน้าที่กำหนดค่าต่างๆ ให้กับพร็อพเพอร์ตี้ของอ็อบเจ็กต์) 

```js
class Car { 
    constructor(param){
		this.param = param; 	// ประกาศพร็อพเพอร์ตี้ param ขึ้นมา (แต่เป็นของอ็อบเจ็กต์) แล้วกำหนดค่าให้มัน
	}
	
	drive(){
		console.log(`The ${this.param} car is running`);
	}
}

let carObj = new Car("red");	// "red"
carObj.drive();					// "The red car is running"
```

#### Property accessors 

เราสามารถมีพร็อพเพอร์ตี้แอคเซสเซอร์ (Property accessors) หรือเมธอด getter กับ setter ในคลาส ดังตัวอย่าง

```js
class Car {
	constructor (){
		this.speedValue = 100; 	
	}
	get speed(){					// เมธอด getter
		return this.speedValue;
	}
   	set speed(speedValue) {			// เมธอด setter
        	this.speedValue = speedValue;
    }
}

let carObj = new Car(100);
console.log(carObj.speed);			// 100

carObj.speed = 60;
console.log(carObj.speed);			// 60
console.log(carObj.speedValue);		// 60 (่ไม่ควรเข้าถึงด้วยวิธีนี้โดยตรง ตามหลัก information hiding ของ OOP)
```

#### Static methods

เมธอดสแตติก (Static methods) คือเมธอดของคลาส ที่เวลาเรียกใช้งานจะต้องผ่านชื่อคลาสโดยตรง (ไม่ต้องเรียกผ่านอ็อบเจ็กต์ เพราะมันไม่ใช่เมธอดของอ็อบเจ็กต์) 

โดยสามารถใช้คีย์เวิร์ด static นำหน้าชื่อเมธอด หรือพร็อพเพอร์ตี้แอคเซสเซอร์ก็ได้ แต่มีข้อแม้ว่าห้ามใช้คำว่า static นำหน้าคอนสตรัคเตอร์ 

```js
class Car {
    constructor (speed){    		// ห้ามมีคำว่า static นำหน้าคอนสตัคเตอร์
        this.speed = speed;
    }
    drive(){            
        console.log("Driving speed:", this.speed);

    }
    static stop() {         		// เมธอดสแตติก
        console.log("Stop this car");
    }
}

// เรียกใช้งานเมธอดสแตติกผ่านชื่อคลาส
Car.stop();             			// "Stop this car"

let carObj = new Car(100);
carObj.drive();         			// "Driving speed: 100"
console.log(typeof carObj.drive);   // "function"
console.log(typeof carObj.stop);    // undefined
```

#### Class Inheritance

การสืบทอดคลาส  (Class Inheritance) ในจาวาสคริปต์ สามารถทำได้โดยใช้คีย์เวิร์ด extends ดังตัวอย่าง

```js
class Calculation {
	constructor (a, b){
		this.a = a;
		this.b = b;
	}
	multiply(){
		return this.a * this.b;
	}   	
}

class Division extends Calculation {	// Division สืบทอดมาจาก Calculation
	constructor (a, b){
		super(a, b);					// เรียกใช้คอนสตรัคเตอร์ของ Calculation
		
		// สามารถกำหนดค่าให้กับ this.a และ this.b ที่อยู่ในคลาสแม่ได้โดยตรง 
		// แต่การทำเช่นนี้จะไม่ปลอดภัย 
		// this.a = a; 	// ไม่ควรทำ	
		// this.b = b;	// ไม่ควรทำ
	}
	
	divide(){
		return this.a / this.b;
	}
}
```

ในตัวอย่างดังกล่าว คลาส Division จะสืบทอดสมาชิก (พร็อพเพอร์ตี้) จากคลาส Calculation ได้แก่ a, b และ multiply โดยเราสามารถเข้าถึงพร็อพเพอร์ตี้เหล่านี้ได้ (ในตัวอย่างถัดไป)

*** ทั้งนี้ในจาวาสคริปต์จะมีเงื่อนไขว่า คอนสตรัคเตอร์ของคลาสลูกต้องเรียก super() ด้วยเสมอ มิฉะนั้นจะเกิด error 

```js
let div = new Division(20,10);

console.log(div.multiply());					// 200
console.log(div.divide());			 			// 2
console.log(div.a, div.b);		 				// 20 10 (ไม่ควรเข้าถึงข้อมูลอ็อบเจ็กต์โดยตรง ด้วยวิธีนี้)

console.log(div instanceof Division);   		// true
console.log(div instanceof Calculation);   		// true
console.log(div instanceof Object);   			// true
```
ให้สังเกต ตอนสร้างอ็อบเจ็กต์ด้วยประโยค new Division(20,10); นอกจากเรียกคอนสตรัคเตอร์ของตัวเองแล้ว (Division)  มันยังเรียกของคลาสแม่ด้วยประโยค super(a, b); ซึ่งจะหมายความว่าให้ส่ง 20 กับ 10 ไปให้คอนสตรัคเตอร์ของ Calculation เพื่อกำหนดค่าให้กับ this.a  และ this.b ตามลำดับ


#### Method overriding
คลาสลูกที่สืบทอดมาจากคลาสแม่ เมธอดของลูกสามารถโอเวอร์ไรด์ (Override)  เมธอดของแม่ได้ด้วย และถ้าเมธอดของคลาสลูกจะเรียกเมธอดของคลาสแม่ (ที่ชื่อซ้ำกัน) ก็ให้เรียกผ่าน super แทน ตัวอย่าง

```js
class Calculation {
	constructor (a, b){
		this.a = a;
		this.b = b;
	}
	multiply(){
		return this.a * this.b;
	}   	
}

class Multiplying extends Calculation {
	constructor (a, b){
		super(a, b);
	}
	multiply(){ 				// โอเวอร์ไรด์เมธอด multiply() ของคลาสแม่
		return "The result is " + super.multiply();
	}   	
}

let m = new  Multiplying(20,10);
console.log(m.multiply());		// "The result is 200" 
```

(บทนี้ ยังไม่เสร็จดีครับ)

### 3.7 Collection
### 3.8 Iterator กับ Generator
### 3.9 Meta Programming
### 3.10 Module
### 3.11 อื่นๆ

## บทที่ 4 แนะนำ ES7

หัวข้อต่อไปนี้จะแสดงฟีเจอร์ใหม่ที่เพิ่มเข้ามาใน ES7 (ECMAScript 2016) รวมทั้งที่เปลี่ยนแปลงไปจาก ES6 ซึ่งมันเปลี่ยนเล็กนิดเดียวเอง

### เพิ่มการใช้งานโอเปอเรเตอร์ยกกำลัง (Exponentiation Operator) 

โอเปอเรเตอร์ยกกำลังจะใช้สัญลักษณ์เป็น ** (ดอกจันสองอันวางติดกัน) เพื่อแทนการคำนวณตัวเลขแบบยกกำลัง โดยไม่ต้องใช้เมธอด Math.pow() ซึ่งจะมีตัวอย่างการใช้งานดังนี้

```js
let ans = 10 ** 2;              			// นำเลข 10 มายกกำลัง 2  ( 102 )
console.log(ans);                      		// 100

// เสมือนใช้เมธอด Math.pow() ดังนี้
console.log(ans === Math.pow(10, 2));     	// true
```

### ลำดับของโอเปอเรเตอร์ **

โอเปอเรเตอร์ ** จะถือว่ามีลำดับความสำคัญสูงกว่าโอเปอเรเตอร์ทางคณิตศาสตร์ตัวอื่น ๆ

```js
let ans = 3 * 10 ** 2;	
console.log(ans);        // 300
```

จากตัวอย่างเดิมจะเสมือนมีวงเล็บมาครอบนิพจน์ (10 ** 2) ดังตัวอย่างซอร์สโค้ดข้างล่าง

```js
let ans = 3 * (10 ** 2);	
console.log(ans);        // 300
```

### ข้อเข้มงวดของโอเปอเรเตอร์ **

โอเปอเรเตอร์ยกกำลังไม่สามารถใช้งานร่วมกับโอเปอเรเตอร์พวก unary expression เช่น - (เครื่องหมายลบ ไม่ใช่การลบ) ,+ (เครื่องหมายบวก ไม่ใช่การบวก), void, delete และ typeof เป็นต้น โดยจะให้ดูตัวอย่างต่อไปนี้ประกอบ

```js
let ans = -10 ** 2; 	// Syntax Error
```

ตัวอย่างที่ยกมานี้จะเกิด error เพราะตรงนิพจน์ -10 ** 2 มันกำกวม เนื่องจากอาจหมายถึง
* -(10  **  2) 
* (-10)  **  2

จากตัวอย่างเดิม ถ้าลองนำวงเล็บมาครอบเพื่อกำหนดลำดับการทำงานเสียใหม่ ก็จะไม่เกิด error ดังตัวอย่าง

```js
let ans = - (10 ** 2); 	// -100
```

จากตัวอย่างเติมเช่นกัน ถ้าลองเปลี่ยนการครอบวงเล็บเสียใหม่ ก็จะได้ผลการทำงานที่แตกต่างกันดังนี้

```js
let ans = (-10) ** 2; 	// 100
```
ขณะเดียวกันโอเปอเรเตอร์ยกกำลังก็จะมีข้อยกเว้น มันสามารถใช้ได้กับ  ++ หรือ -- (เป็น unary expression) โดยไม่ต้องใช้วงเล็บครอบ
ลองพิจารณาการใช้โอเปอเรเตอร์ยกกำลังร่วมกับโอเปอเรอเตอร์ ++ ดังตัวอย่าง

```js
let value1 = 9, value2 = 10;

// ใช้งานโอเปอเรเตอร์ ++ แบบ prefix
// ค่าของ value1 ถูกบวกด้วยหนึ่ง ก่อนที่จะยกกำลัง 2 
console.log(++value1 ** 2);     // 100
console.log(value1);            // 10 

// ใช้งานโอเปอเรเตอร์ ++ แบบ postfix
// หลังจากยกกำลัง 2 ไปแล้ว ค่าของ value2 จึงถูกบวกด้วยหนึ่งทีหลัง
console.log(value2++ ** 2);     // 100
console.log(value2);            // 11
```

ลองพิจารณาการใช้โอเปอเรเตอร์ยกกำลังร่วมกับโอเปอเรเตอร์  -- ดังตัวอย่าง

```js
let value1 = 11, value2 = 10;

// ใช้งานโอเปอเรเตอร์ -- แบบ prefix
// ค่า value1 ถูกลบด้วยหนึ่ง ก่อนที่จะยกกำลัง 2 
console.log(--value1 ** 2);     // 100
console.log(value1);            // 10 

// ใช้งานโอเปอเรเตอร์ -- แบบ postfix
// หลังจากยกกำลัง 2 ไปแล้ว ค่าของ value2 จึงถูกลบด้วยหนึ่งทีหลัง 
console.log(value2-- ** 2);     // 100
console.log(value2);            // 9
```

### เพิ่มเมธอด Array.prototype.includes()

สำหรับ ES6 นั้น สตริงทุกตัวจะมีเมธอด includes() และเช่นเดียวกันใน ES7 ก็ได้เพิ่มเมธอดดังกล่าวให้กับอาร์เรย์ โดยมีจุดประสงค์ใช้ค้นหาข้อมูลในอาร์เรย์ ถ้าเจอข้อมูลที่ต้องการหาก็จะรีเทิร์นเป็น true ถ้าไม่เจอก็จะได้เป็น false ดังตัวอย่าง (ทำงานแบบเดียวกับ includes() ของสตริงบทที่ 5 ในหนังสือ [1])

```js
let array = ["A", "B", "C"];        		// ประกาศอาร์เรย์

console.log(array.includes("A"));         	// true
console.log(array.includes("Z"));         	// false
```

ในตัวอย่างนี้จะค้นหาตัวอักษร "A" เจอในอาร์เรย์ แต่ไม่สามารถค้นหา "Z" พบ เพราะมันไม่มีอยู่ในอาร์เรย์
ปกติแล้วเมธอด includes() จะเริ่มค้นหาที่ตำแหน่งอินเด็กซ์เป็น 0 โดยดีฟอลต์ ดังนั้นถ้าจะเปลี่ยนตำแหน่งอินเด็กซ์ที่ใช้ค้นหา ก็สามารถทำได้ดังตัวอย่าง

```js
let array = ["A", "B", "C"];        		// ประกาศอาร์เรย์

// เริ่มค้นหา "B" จากอินเด็กซ์คือ 2 ซึ่งจะพบว่าหาไม่เจอ
console.log(array.includes("B", 2));        // false

// แต่ถ้าเปลี่ยนมาเริ่มค้นหาจากอินเด็กซ์เป็น 1 ก็จะหา "B" เจอ
console.log(array.includes("B", 1));        // true
```
ในตัวอย่างดังกล่าวจะเห็นว่าเมธอด includes รับค่าอากิวเมนต์ตัวที่สอง เพื่อระบุตำแหน่งเริ่มต้นของอินเด็กซ์ที่จะใช้ค้นหาข้อมูลในอาร์เรย์

### ข้อควรระวัง includes()

เมธอด includes() จะเสมือนใช้โอเปอเรเตอร์ === เปรียบเทียบว่ามีสมาชิกที่ต้องค้นหาหรือไม่ แต่ทว่าเวลามันเห็นข้อมูลเป็น NaN ก็จะมองว่ามีค่าเท่ากัน (เปรียบเทียบแล้วได้ true)  ซึ่งจะแตกต่างจาก indexOf ซึ่งจะเสมือนใช้ === เช่นกัน ซึ่งเวลามันเห็น NaN จะมองว่ามีค่าต่างกัน (เปรียบเทียบแล้วได้ false) ดังตัวอย่าง

```js
let array = [0, NaN, 1];

console.log(array.indexOf(NaN));       // -1    -- ไม่เจอสมาชิกที่ต้องการ
console.log(array.includes(NaN));      // true
```

แต่ถ้าข้อมูลเป็น +0 กับ -0 จะมองว่าเท่ากัน (เปรียบเทียบแล้วได้เป็น true) ทั้ง includes() กับ indexOf() ดังตัวอย่าง

```js
let array = [-0, NaN, 1];

console.log(array.indexOf(+0));       // 0	 -- เจอค่า -0 อยู่ในอาร์เรย์ที่ตำแหน่งอินเด็กซ์ 0
console.log(array.includes(+0));      // true
```

### TypedArray.prototype.includes()

ในอาร์เรย์ระดับบิต (TypedArray บทที่ 12 ของหนังสือ [1]) ก็จะมีเมธอด includes() ให้ใช้งานเหมือนกับอาร์เรย์ในหัวข้อก่อนหน้านี้ทุกประการเด๊ะ ดังตัวอย่าง

```js
let uint8 = new Uint8Array([1, 2, 3, 4, 5]);

console.log(uint8.includes(1));     	// true
console.log(uint8.includes(5));     	// true
console.log(uint8.includes(10));     	// false
```

### สิ่งที่เปลี่ยนแปลงไปของ ES7 เมื่อเทียบกับ ES6 (นิดเดียวเอง)

หัวข้อก่อนหน้านี้ได้กล่าวถึงฟีเจอร์ที่เพิ่มมาใหม่ใน  ES7 แต่หัวข้อนี้จะกล่าวถึงฟีเจอร์ที่เปลี่ยนไปจาก ES6 ดังนี้

* trap ที่เป็น enumerate() ของพร็อกซี่ (บทที่ 14 ของหนังสือ [1]) ถูกเอาออกไปใน ES7 เรียบร้อยแล้ว
* เจอเนอเรเตอร์ (บทที่ 13 ของหนังสือ [1]) ไม่มี [[Construct]]  ถ้าเรียก new จะเกิด error ขึ้นมาดังตัวอย่าง

```js
function * generator() {}
let iterator = new generator(); 	// throws "TypeError: f is not a constructor"
```

## บทที่ 5 แนะนำ ES8 (ยังไม่เสร็จ)

สิ่งที่คาดว่าจะเพิ่มเข้ามาใน ES8 (ECMAScript 2017) (มีนิดเดียว)

* Object.values() 
* Object.entries()

## อ้างอิง

* [1] หนังสือ “พัฒนาเว็บแอปพลิเคชั่นด้วย JavaScript” จะอธิบายถึงมาตรฐานตัวใหม่ ECMAScript 2015 หรือเรียกสั้น ๆ ว่า “ES6” หรือ “ES6 Harmony” โดยเล่มนี้ตีพิมพ์และจัดจำหน่ายโดยซีเอ็ด
* [2] https://developer.mozilla.org/en-US/docs/Web/JavaScript/
* [3] https://github.com/nzakas/understandinges6/blob/master/manuscript/B-ECMAScript-7.md
* [4] http://www.ecma-international.org/ecma-262/7.0/
* [5] https://tc39.github.io/ecma262/
* [6] https://github.com/google/traceur-compiler/wiki/Getting-Started
* [7] https://github.com/babel/babel-standalone
* [8] http://exploringjs.com/es6/
* [9] https://leanpub.com/exploring-es2016-es2017/read
* [10] https://leanpub.com/setting-up-es6/read#sec_es6-repls
* [11] https://leanpub.com/ecmascript2015es6guide/read
* [12] https://leanpub.com/understandinges6/read
* [13] https://github.com/nzakas/understandinges6/tree/master/manuscript


## ทิ้งท้าย

เหตุผลที่เขียนบทความชุดนี้ เพราะหลังจากเขียนหนังสือ ดังกล่าวไปแล้ว (ตามรูปข้างล่าง) เทคโนโลยีจาวาสคริปต์ก็ดูเหมือนพัฒนาต่อเนื่อง (ยังไม่นิ่ง)
ด้วยเหตุนี้ ....

* เนื้อหาทั้งหมดต่อไปนี้ จะเหมือนเป็น**ภาคต่อ**จากหนังสือดังกล่าว
* จะทบทวนจาวาสคริปต์ตามมาตรฐานเก่า ES5 นิดหน่อยให้เห็นภาพ ไม่ลงรายละเอียดลึก
* จะเป็นการพาทัวร์ภาษาจาวาสคริปต์ (JavaScript) ยุคสมัยใหม่ตามมาตรฐาน ES6 คร่าวๆ ให้เห็นภาพ ไม่ลงรายละเอียดลึก
* จะพูดถึงภาษาจาวาสคริปต์ (JavaScript) ยุคสมัยใหม่ตามมาตรฐาน ES7, ES8 (ไม่มีในหนังสือ)
* รวมทั้งเพิ่มเนื้อหาที่ไม่อยู่ในหนังสือ (คือตอนแต่งหนังสือ เทคโนโลยีต่างๆ ยังไม่อื้ออำนวย ผมเลยไม่กล้าเขียนลงไปครับ)
* **ทั้งนี้เนื้อหาจะต่างจากหนังสือข้างต้น ไม่เหมือนกันเท่าไร**
* **เขียนยังไม่เสร็จดี** กะว่าจะทยอยเขียนไปเรื่อยๆ (ถ้ามีเวลาว่าง) ซึ่งถ้าได้ปริมาณมากพอ อนาคตอาจมีรวบรวมทำเป็นเล่ม 2 เพื่อวางขายต่อไป

*** ใครเอาเนื้อหาผมไปใช้ โปรดให้เครดิตลิงค์ต้นฉบับต้นด้วยนะคร๊าบบบบบ

ถ้าสนใจข่าวสารไอที ทั้งสาระบ้าง และไร้สาระบ้าง ก็ตามได้ที่

* https://www.facebook.com/programmerthai/

สามารถให้คำชี้แนะ คอมเมนต์ และฟีดแบ็คผมได้ตลอดเวลา ที่

* http://www.patanasongsivilai.com/javascript.html


## สำหรับผู้ที่สนใจหนังสือเล่มนี้

หนังสือ__ภาษาไทยเล่มแรก__ที่กล่าวถึงจาวาสคริปต์มาตรฐานใหม่ พิมพ์ครั้งที่สองแล้วนะครับ มีการปรับปรุงแก้ไขคำผิดไป **แต่ทว่าตีพิม์จำนวนจำกัด ไม่มากเท่าไร** มีขายบางแห่งเท่านั้น ควรเช็คผ่านกูเกิลอีกทีว่าที่ไหนมีขายบ้าง

![cover](images/cover_big5.png)

* [ศูนย์หนังสือจุฬา]( http://www.chulabook.com/description.asp?barcode=9786160825394)
* [ร้านนายอินทร์](https://www.naiin.com/product/detail/191081/)
* [ร้าน Book Smile](http://www.booksmile.co.th/คอมพิวเตอร์อินเทอร์เน็ต/พัฒนาเว็บแอบพลิเคชั่นด้วย-JavaScript.html)
* [ร้าน kinokuniya thailand](https://thailand.kinokuniya.com/bw/9786160825394)
* [ผ่านฟ้าบุ๊คเซ็นเตอร์] (http://www.phanpha.com/item/พัฒนาเว็บแอปพลิเคชั่นด้วย-javascript)
* [ซีเอ็ดบางสาขา]( https://www.se-ed.com/product/พัฒนาเว็บแอปพลิเคชั่นด้วย-JavaScript.aspx?no=9786160825394)
* และร้านหนังสืออื่น ๆ ที่ไม่ได้กล่าว
