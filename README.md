# phpcaptcha

This is a very simple php code to put captcha on your form.

What your have to do is put this captcha.php file on your file system and put this code: 
`<img src="captcha.php" />`
wherever you want to put the captcha.

You have to use a `<input type="text" name="captcha" />` field also which you use for matching the characters showing in the captcha image. Then put this condition on your form handler code

```javascript
if(isset($_POST["captcha"])&&$_POST["captcha"]!=""&&$_SESSION["code"]==$_POST["captcha"]){
  do whatever your want to do man

}
```
