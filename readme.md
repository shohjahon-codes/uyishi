# **Dars-8** <p>*Mavzu:* **Funcsiya , funcsiyanig asosiy 3 ta turi :**</p> <p>*- Function declaration*</p> <p>*- Function expession*</p> <p>*- Arrow function*</p>

## 1.  F U N C T I O N S 
 -  *Funksiya - JavaScript dasturlash tilining asoslaridan biri bo'lob uning yordamida malum bir vazifani bajarish mumkun . Funksiya boshqa bir kod qismida chaqirilganda ishga tushadi . Funksiya yordamida kodni qayta ishlatishlik imkoni mavjud yani birmarotaba elon qilib , bir necha joyda ishlatishlik imkoni mavjud , o'hshati lozim bo'lsa SCSS degi mixsend larga qisman o'hshab ketadi .*

<p>Sintactisti quydagicha :</p>

 ```
 function square(number) {
  return number * number;
}

 ```

<p>M:</p>

```
function power(a,n){
    let b = a**n;
    return b
}

console.log(power(3,2));

// natija ==> 9 
```
### *Function declaration*
- *Funktsiya deklaratsiyasi nima?
Funktsiya deklaratsiyasi funktsiyani belgilaydigan identifikatorni kiritadi va ixtiyoriy ravishda funktsiya parametrlarining turlarini (prototipi) belgilaydi. Funktsiya e'lonlari (ta'riflardan farqli o'laroq) fayllar ko'lami bilan bir qatorda blok doirasida ham paydo bo'lishi mumkin.*

- *Funktsiya declaration qolganlaridan  yanabir kuchli farqi uni elon qilib olganimazdan so'ng istalgan joyda chaqirib ishlata olamiz hatto funksiya elongqilingan satirdan yuqorida chaqirib ham !*

<p>M :</p>

```
function sonBoluvch(n) {
    for (let i = 1 ; i < n ; i++) {
        if(n % i == 0){
            console.log(i);
        }
    }
}
sonBoluvch(10);
```

### *Function expession*
- *Function expession sintaksis jihatdan huddi declaration ohshaydi , asosiy farq bu funksiya nomi bo‘lib yani declarationda biz funcsiyaga nim bergan bo'lsak bunda o'zgaruvchi elon qilib unga funcsiyani elon qilib ketamiz va chaqirib olishda shu o'zgaruvchi nomi bilan chaqirib olamiz , yana bir asosiy farqi uni o'zidan yoqorida chaqira olmaymiz !*

- *Function expession afzalig jihatilaridan biri shuki unu yan ihtiyori bir ozgaruvchiga tenglab , ihtiyoricha o'zlashtirib ishlatishligimiz mumkun , buni 2- misolda ko'rsak yanayam tushunarliroq bo'ladi !*

<p>M :</p>

```
const funcNam = function () {
    console.log("Lesson - 8");
}

funcNam(); // natija ==>  Lesson - 8

// -------------- 2 - misol -----------------

const funcNam = function (a , b) {
    console.log(a+b);
}

funcNam(4,6); // natiga ==> 10

let test = funcNam ;

test(20,67); // ===>  87 
```

### *Arrow function*

- *Arrow function hozirgacha ko'rgan funcsiyalarimiz ichida va umumiy jihatda eng ko'p ishlatladigan funcsiya bo'lib hisoblanadi u ishlash jihatidan avalgi korganlarimiz bilan birhiln ish bajaradi sintacsistida biroz far qiladi unin misolda ko'rsak yanayam tushunarliroq bo'ladi.*

- *Arrow function yana bir avzalligi uni stentminti birdona bo'ladigan bo'lsa uni hechqanday bloc skoplarsiz yan <b>" { } "</b>  yai figurni qavuslarsiz bir qatorning o'zida yozib ketsak ham boladi <b>1- misolda</b> ko'rishligimiz mumkun*

<p>M :</p>

```
// ---------  1- misol  -------

const funcNam = () => console.log("hello");

funcNam(); // natija ===> hello

// -------- 2 misol--------------------------

const funcNam = (a, b , c) => {
    if(a>b && b>c){
        console.log(a+b/c);
    }else{
        console.log(a+b+c);
    }
};

funcNam(20,12,4); // natija ==> 23
```