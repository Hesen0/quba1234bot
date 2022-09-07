import telebot
import emailCheck
bot_token = '5457685629:AAGKlR3jw-N-lRbWmKEXrIcJmzSBbzLi8xw'
email = []
MailDataFile = open('F:\Hasan\MailData.txt',"a+")
MyBot = telebot.TeleBot(bot_token)
@MyBot.message_handler(commands=["start"])
def Start(message):
    MyBot.reply_to(message,"Xos geldiniz")

@MyBot.message_handler(func=lambda message: True)
def UserMessage(message):
    UserInput = str(message.text).lower()





while True:
    try:
        MyBot.polling()
    except Exception:
        MyBot.polling()
