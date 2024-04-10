from pyrogram import Client, filters, types

api_id = 21853778 #API_ID : https://my.telegram.org/
api_hash = "48916f2c681773a7bf527593ada2e055" #API_HASH : https://my.telegram.org/

app = Client("#iCoderNet", api_id, api_hash)


@app.on_message(filters.channel)
async def replyComment(client, message: types.Message):
    chat_id = message.chat.id
    message_id = message.id
    try:
        msg = await app.get_discussion_message(chat_id, message_id)
        await msg.reply("1")
    except:
        pass

app.run()
