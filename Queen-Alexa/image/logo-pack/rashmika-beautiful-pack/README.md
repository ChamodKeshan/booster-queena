# RASHMIKA MANDANA

CREATED WITH ChamodKeshan. POWER FULL USE WITH [Queen-Alexa](https://github.com/ChamodKeshan/Queen-Alexa) WA BOT PROJECT.
 # EXAMPLE
````
const Alex = require('../events');
const {MessageType, MessageOptions, Mimetype} = require('@adiwajshing/baileys');
const axios = require('axios');
const Config = require('../config');

    Alex.addCommand({pattern: 'rashmika', fromMe: true, desc: 'random rashmika images'}, (async (message, match) => {

    var r_text = new Array ();

r_text[0] = "https://raw.githubusercontent.com/ChamodKeshan/booster-queena/master/Queen-Alexa/image/logo-pack/rashmika-beautiful-pack/1655255595284.jpg";
r_text[1] = "https://raw.githubusercontent.com/ChamodKeshan/booster-queena/master/Queen-Alexa/image/logo-pack/rashmika-beautiful-pack/1655255615700.jpg";
r_text[2] = "https://raw.githubusercontent.com/ChamodKeshan/booster-queena/master/Queen-Alexa/image/logo-pack/rashmika-beautiful-pack/1655255625496.jpg";
r_text[3] = "https://raw.githubusercontent.com/ChamodKeshan/booster-queena/master/Queen-Alexa/image/logo-pack/rashmika-beautiful-pack/1655255641443.jpg";
r_text[4] = "https://raw.githubusercontent.com/ChamodKeshan/booster-queena/master/Queen-Alexa/image/logo-pack/rashmika-beautiful-pack/1655255649080.jpg";
r_text[5] = "https://raw.githubusercontent.com/ChamodKeshan/booster-queena/master/Queen-Alexa/image/logo-pack/rashmika-beautiful-pack/1655255724397.jpg";

var i = Math.floor(6*Math.random())

    var respoimage = await axios.get(`${r_text[i]}`, { responseType: 'arraybuffer' })

    await message.sendMessage(Buffer(respoimage.data), MessageType.image, {mimetype: Mimetype.png, caption: 'made with Alexa'})

    }));
}
````
