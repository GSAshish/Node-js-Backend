
crypto is for creating unique

built in crypto library

```js
const crypto=require("crypto");
crypto.randomBytes(32,(err,byffer))=>{
if(err){
// throw and redirect back
}
const token=buffer.toString("hex");

user.find({email,password}).then((user)=>{
              user.resetToken=token;					    user.resetTokenExpiry:Date().now()+3600000;
										 })
}


// donot forgot to add resetToken and resetTokenExpiry
```