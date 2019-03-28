# P210-28032019-JSON_Forms

Dersde baxilan linkler:

- https://www.w3schools.com/js/js_json.asp 
- https://www.w3schools.com/js/js_validation.asp
- https://www.w3schools.com/js/js_validation_api.asp
- https://www.w3schools.com/js/js_object_definition.asp
- https://www.w3schools.com/js/js_object_properties.asp
- https://www.w3schools.com/js/js_object_methods.asp
- https://www.w3schools.com/js/js_object_accessors.asp
- https://regexr.com/


## Tapshiriq
Yeni istifadecinin melumatlarini daxil etmek ucun form yaratmalisiniz. Form 4 inputdan ibaret olmalidir:
1. Name
2. Surname
3. Birthday
4. Email

Butun inputlarin type-i text olsun.

Form submit olunanda yoxlanilmalidir:
- Inputlarin hec biri bosh olmasin
- Name ve Surname inputlari yalniz herfler qebul etsin
- Birthday inputu ISO standardina uygun formatda il, ay ve gun qebul etsin
- Email inputu duzgun formatda email qebul etsin.

Eger form submit olunanda validation proseduru ugurlu kecerse JavaScript hissede yeni bir Person instance-i yaradib, yaradilmish instance-i "persons" array-ine daxil edin. Person object-inin structuru ashagidaki kimi olmalidir:

- Person
    - Properties:
        - id : number
        - name : string
        - surname : string
        - birthday : string
        - age : number
        - email : string
    - Methods:
        - calculateAge()

Inputlardan gelen melumata esasen yeni object yaratmaq lazimdir. Birthday inputundaki tarixe uygun calculateAge methodunu istifade ederek age propertisine de value vermek lazimdir.
Proses ugurla basha catdiqdan sonra "persons" array-indeki istifadecileri ekranda list sheklinde gostermek lazimdir ve formdaki inputlarin ici temizlenmelidir.

Siyahida istifadecinin melumatlari bu shekilde gosterilmelidir:

    - id. name surname age email

Siyahinin uzerinde ise istenilen list item-i sile bilmek ucun istifadecinin ID-sini yaza bileceyimiz bir input ve delete button-u qoyun. Siyahidaki her hansi bir istifadecinin ID-sini yazdiqdan sonra delete button-una click etdikce onu silmish olum. Eger ID inputuna number tipinden bashqa birshey daxil olunarsa ve ya siyahida olmayan bir ID daxil olunarsa validation ile yoxlayib error gostermek lazimdir.

Istifadecilerin melumatlarini gosteren siyahinin ust hissesinde 3 eded button olmalidir. Bunlar Id, Name ve Surname uzre siralamani yerine yetirmelidirler. Yeni, eger Name buttonuna click edilerse siyahi istifadecilerin adlarina uygun siralanmalidir. Eger Id buttonuna click edilerse istifadecilerin Id nomresine uygun siralanmalidir. Eger Surname buttonuna click edilerse istifadecilerin soyadlarina uygun siralanmalidir. 


QEYD: HTML hissede hec bir validasiya attributundan (meselen required, min, max ve s) istifade etmeyin.
