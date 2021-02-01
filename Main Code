const kalingModule = require('kaling').Kakao();
const Kakao = new kalingModule();
Kakao.init(''); //자스키
Kakao.login('',''); //아디•비번

var m = [];

function response(room, msg, sender, isGroupChat, replier, ImageDB, packageName, threadId) {


if (msg.startsWith(".카링 ")) {
  m = msg.substr(4).split("+");
  try {
    //replier.reply(m);
    
Kakao.send(room, {"link_ver" : "4.0",
                  "template_id" : 45883,
                  "template_args" : {
                    a: m[0],
                    b: m[1],
                    Img: m[2]
                 }
                 }, "custom");

} catch(e) {
  replier.reply(e);
}

}
} 
