import datetime

def birthday_wish(name):
    today = datetime.date.today()
    if today.month == 8 and today.day == 23:
        print(f"亲爱的{name}，没想到吧？哥还有这方面的才华。不愧是我。又到了一年一度的颖哥幸福日，在这里哥为你献上 24 小时的祝福：生日快乐！岁月匆匆，但我们的友谊从未褪色。回想起一起走过的时光，那些欢笑、泪水、打闹和陪伴，都成为了生命中最珍贵的宝藏。新的一岁，愿你拥有更多的勇气去追求自己的热爱，无论风雨还是晴空，我都会一直在你身边。愿你的生活如诗如画，愿你的心情如春花般灿烂，愿你的未来光芒万丈！")
    elif today.month == 8 and today.day < 23:
        days_until_birthday = 23 - today.day
        print(f"亲爱的{name}，还有{days_until_birthday}天就到你的生日啦，期待那美好的一刻！")
    elif today.month == 8 and today.day > 23:
        print(f"亲爱的{name}，你的生日已经过去了，但祝福永远不会迟到，愿你新的一岁美好常伴！")
    else:
        print("还没到生日的时间哦，耐心等待！")

name = "颖哥"
birthday_wish(name)
