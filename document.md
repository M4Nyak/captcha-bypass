# captcha-bypass
I will teach you professional captcha bypass

first we should download https://github.com/capsolver/capsolver-python after we will write import capsolver and enter our api key we will get api key from https://dashboard.capsolver.com/dashboard/overview after we will write
capsolver.api_key="your capsolver api key"
solution = capsolver.solve({
        "type":"",
        "websiteKey":"",
        "websiteURL":"",
    })
now i will tell what is that things
first we will take captcha value we will press f12 and "we will https://recaptha...k="take this value" and print this to websitekey 

solution = capsolver.solve({
        "type":"",
        "websiteKey":"the value after https://recaptha...k= ",
        "websiteURL":"https://website.com",
    })


  and now i will tell what is type. It s mean what we bypassing which captcha
  first we will enter capsolver website after click createtask after click view all supported... after there will be two recaptcha and they are proxyless and proxy. I will explain proxyles one week after i will explain with proxy recaptcha. we will write type 
  solution = capsolver.solve({
        "type":"ReCaptchaV2TaskProxyless",
        "websiteKey":"the value after https://recaptha...k= ",
        "websiteURL":"https://website.com",
    })
    now print(solution) will bypass recaptcha





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

now we should get the thing we want do
now press f12 and after we must find the element of button we want click (not recaptcha) and we will right click and copy xpath
value1= agac.xpath("xpathvalue")
value2= agac.xpath("otherxpathvalue")
and now
print(value1)
print(value2)
and it will solve





 -Ömovsky
