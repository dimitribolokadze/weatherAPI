OpenWeatherMap API-ის გამოყენებით მოაქვს თბილისის ამინდის 5 დღის პროგნოზი, 3 საათიანი ინტერვალებით. 

გამოვიყენე რამდენიმე ბიბლიოთეკა, requests (HTTP რექვესთებისთვის), json, datetime (მიღებული მონაცემების ფორმატირებისთვის), win10toast import ToastNotifier (ნოტიფიკაციისთვის). 

პირველად ვამოწმებთ if/else -ით თუ რესფონსი წარმატებით დასრულდა, პროგრამა წამოიღებს ამინდის მონაცემებს. 
თუ რესფონსი წარმატებულია, ის აანალიზებს JSON მონაცემებს პასუხში json.loads() მეთოდის გამოყენებით,  ობიექტს  weather_data. 
შემდეგ ინახავს მონაცემებს JSON ფაილში json.dump()-ის გამოყენებით. 

საბოლოოდ ნოტიფიკაციისთვის აჩვენებს ToastNotifier მოდულის გამოყენებით
    
# P.S ნოთიფიკაცია არ მომსვლია 2 ქვიზის და სულ გადამავიწყდა მეორე ქვიზის ატვირთვა :( 
# მესამე და მეორე ქვიზს ერთად ვტვირთავ დღეს 14.05
