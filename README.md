import telebot


bot = telebot.TeleBot("7860150670:AAHD-ZdlubEQcEe1MyenC0W66IkJoQheBhi")


@bot.message_handler(content_types=['text'])
def send_echo(message):
    bot.send_message(message.chat.id, message.text)


bot.polling(none_stop=True
#ОНО НЕ РАБОТАЕТ КЛАСС😭
