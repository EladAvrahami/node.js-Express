# node.js + Express proj
### start+ sum node.js and Express framwork important subj

## General / Terminal commands:
#### Download latest express version  :
terminal -> npx express --hbs -> npm install
#### Terminat process  :
cntrl+ c
#### copy line shortcut:
alt+shift+arrowDown/UP
#### PAY ATTENTION : THE FIRST PAGE WILL ALWAYS CALLED index.html


## part 11 - VIP  Person Proj
### get out index with for loops in hbs file 
{{#if}} -if בתוך הנדל ברס  בדיקה האם קיים מאפיין מסויים בגייסון/מערך, אם לא מוצא את המאפיין תבצע את הפעולה  </br>
{{else}} - שים לב שנכתב בתוך ה if </br> 
{{#each _ar}} - לכתיבת אובייקטים עי מעבר על מערך באמצעות דאבל אינקפסולשיין בלולואת each </br>
{{#unless worth}} - מבצע פעולת איף הפוכה כלומר במידה ומצא מאפיים בגייסון לדוגמא יבצע את הפעולה </br>
{{@index}} - find ob index 

## part 12 - VIP Person Proj
###   routing by url + collect prams from url 
router.get('/', function(req, res, next) { - router will effect on the location by url</br>
res.render (...)}  - render will tell me to start hbs file </br>
router.get('/:id_vip', function(req, res, next) { - נרשום נקודותיים לפני המאפיין שבגרשיים עמ שיבין שלא מדובר בהפנייה לתקייה אלא בפרמטר

## BITCOIN_Project
###   routing by url + collect prams from url 
###   work with api +loops in incupsolation+menipulate json data in order to show on HBS files
1.Download Axios . </br>
*bit.hbs file - in order to choose spesific coin from coin array api i willl write : {{array.0.name}} </br>
so the array- is a parameter that contain my json data, 0- is the index of the obj in that json api , and name - will be one an attribute in that json obj</br>
2. Add bootstarp link to the general layout.hbs file.  from ->https://getbootstrap.com/docs/5.1/getting-started/download/</br>
3. menipulate respons data in the index js file and use it on bit.hbs file </br>
4. PAY ATTENTION : SERVER PORT 3001 + ADD TO URL "/bit"


## Project 3 
### 1. Middleware 
</br>
  create API + set the Middleware (JSON parsing + static files) and public folder +AppRouting
הגדרת תקיית פובליק כתקייה סטטטית שניתן לשים בה קבצים לצד לקוח ולצד לקוח יהיה גישה </br>  
כוח מטורף מבחינת ראוטינג כי גם יחסוך לי פעולת גט לכל קובץ בתקיית פובליק וגם יזהה אוטומטית קבצים שנמצאים בפובליק
בניסיון להגיע אליהם בשורת הכתובת בתצוגת המשתמש : </br>
app.use(express.static(path.join(__dirname,"public")));

-----------------------------------------------------------------------------------

### 2. Order my routes
open new file called  "confige_routes" and do export to it 
using the middelware **" .use "** on the config_routes file in order to get a path to get the url of the indexRout for instance...

app.use("/users",usersRout) wiil ref to useresRout file and in it will be more part of the url like in this example:

router.get("/user1",(req,res)=>{
     //יחזיר מידע בפורמט גייסון שאני הגדרתי על המסך בשם הודוע 
     res.json({msg:"USERS ROUT WORK 4444"})
})

### 3. Create Query string
shopRout file ...

### 4. Connect to mongoDB 
https://mongoosejs.com/docs/index.html - quick start guide </br>
add require("./db/ConnectMongo") to app.js file

### 11.8 craete schema as a modele of collection (like interface)

/*create some kind of interface to avoid Multiple keys */</br>
const foodSchema = new mongoose.Schema({</br>
name:String,</br>
img:String,</br>
cak:Number,</br>
price:Number</br>
});


### linkes for tommorow: 
https://www.bezkoder.com/node-js-express-sequelize-mysql/ (include video)</br>
https://www.bezkoder.com/node-js-rest-api-express-mysql/ regular(main)</br>
https://github.com/atrem13/restful-api-express-mysql-bezcoder-  code example 

<!--  https://monkeys.co.il/  -->








