# captcha-bypass
Ben size profesyonel captcha bypass'ı öğretirim

öncelikle https://github.com/capsolver/capsolver-python'u indirelim sonra import capsolver yazıp api keyimizi gireceğiz https://dashboard.capsolver.com/dashboard/overview adresinden api key alacağız sonra yapacağız capsolver.api_key="your capsolver api key" solution = capsolver.solve({ "type":"", "websiteKey":"", "websiteURL":"", }) yazın, şimdi önce bunların ne olduğunu anlatacağım captcha değerini alacağız f12'ye basacağız ve " https://recaptha...k=" bu değeri alacağız" ve bunu websitekey'e yazdıracağız

çözüm = capsolver.solve({ "type":"", "websiteKey":" https://recaptha...k='den sonraki değer ", "websiteURL":" https://website.com ", })

ve şimdi türün ne olduğunu söyleyeceğim. Bu, hangi captcha'yı atladığımız anlamına gelir, önce captcha'yı tıkladıktan sonra capsolver web sitesine gireceğiz, tıkladıktan sonra oluştur, tümünü görüntüle desteklenir... sonra iki recaptcha olacak ve bunlar proxy'siz ve proxy'dir. Proxy recaptcha ile anlatacağımdan bir hafta sonra proxyleri anlatacağım. type solution = capsolver.solve({ "type":"ReCaptchaV2TaskProxyless", "websiteKey":" https://recaptha...k= " dan sonraki değer ", "websiteURL":" https://website yazacağız . com ", }) şimdi yazdır(çözüm) recaptcha'yı atlayacak

now i will tell how we can use that with requests module
first we will open requests.session
s=requests.session()
s.headers={
"your user agent"
}
r= s.get("website.com")
print(s.cookies.get_dict())
#we should import html from lxml
from lxml import html
agac= html.fromstring(r.content)
şimdi yapmak istediğimiz şeyi almalıyız şimdi f12'ye basın ve sonra tıklamak istediğimiz (recaptcha değil) butonun elemanını bulmalıyız ve sağ tıklayıp xpath value1= agac.xpath("xpathvalue") value2= agac'ı kopyalayacağız. xpath("otherxpathvalue") ve şimdi print(value1) print(value2) ve çözecek

-Ömovski
