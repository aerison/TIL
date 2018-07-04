https://api.telegram.org/bot577998246:AAHYLNWbZlQQlj3L34K4BMbvPhCAJeZFD14/getUpdates



https://api.telegram.org/bot+(token)



치면, ok true볼 수 있움!



콘솔에서, irb

```console
2.4.0 :016 >   res_json['result'][0]
 => {"update_id"=>311123204, "message"=>{"message_id"=>3, "from"=>{"id"=>593710174, "is_bot"=>false, "first_name"=>"aeri", "last_name"=>"son", "language_code"=>"ko-KR"}, "chat"=>{"id"=>593710174, "first_name"=>"aeri", "last_name"=>"son", "type"=>"private"}, "date"=>1530667745, "text"=>"hey"}} 
2.4.0 :017 > res_json['result'][0]['message']
 => {"message_id"=>3, "from"=>{"id"=>593710174, "is_bot"=>false, "first_name"=>"aeri", "last_name"=>"son", "language_code"=>"ko-KR"}, "chat"=>{"id"=>593710174, "first_name"=>"aeri", "last_name"=>"son", "type"=>"private"}, "date"=>1530667745, "text"=>"hey"} 
2.4.0 :018 > res_json['result'][0]['message']['id']
 => nil 
2.4.0 :019 > res_json['result'][0]['message']['from']
 => {"id"=>593710174, "is_bot"=>false, "first_name"=>"aeri", "last_name"=>"son", "language_code"=>"ko-KR"} 
2.4.0 :020 > res_json['result'][0]['message']['from']['id']
 => 593710174 
2.4.0 :021 > 
```

https://core.telegram.org/bots/api

메세지ㅏ로 보내는 것.....

```console
july0325:~/workspace (master) $ ruby telegram.rb 2&>> t.txt
july0325:~/workspace (master) $ ruby telegram.rb 2&>> t.txt
july0325:~/workspace (master) $ ruby telegram.rb
/watch?v=inYELxTgFR4
/watch?v=6929As3YK-s
/watch?v=yGU2SfH5pUM
/watch?v=jgqmPWKscuI
/watch?v=bLcZpsJp21M
/watch?v=NlrIWrHSqRk
/watch?v=kcqnBsdq59E
/watch?v=pUbrigDMV3A
/watch?v=8RYkFuUQMjw
/watch?v=IwygN_g_aKA
/watch?v=uXVScLWIS74
/watch?v=JC-IG-tBctU
/watch?v=JRaQM0aBtVM
/watch?v=6P5N5uYwACE
/watch?v=U-HshygKZkk
/watch?v=keh9bwK4Guk
/watch?v=UwZuxmuN-Qw
/watch?v=exftKarulWg
/watch?v=vPnTmrGZllk
/watch?v=Fc0IxMgBZ-E
/watch?v=-AccJni925g
/watch?v=IOLfynoR9NQ
/watch?v=RRhTw9jbGRo
/watch?v=ZmgmVY7a1JY
/watch?v=SO2S7-Ygf4c
/watch?v=I0x7EHzKQW0
/watch?v=XlmOtC6Uhgk
/watch?v=q7szVxDh5ZM
/watch?v=I9s-GcdkfOQ
/watch?v=WhQPcDs_qWo
소행성 표류기 🌊 수영장에서 대형튜브로 신나게 놀아요 🐥
심쿵주의 🌸 대형견에게 푹 안기는 소형견 🐰 소녀사랑행성 💕
감당안되는 대형견들의 체력...ㄷㄷ 리트리버 특공대 🐕
귀여움끝판왕 🐶 간식이 좋아서 발동동 구르는 강아지
Watermelon 🍉 Real Sound 🌊 Dog ASMR Mukbang Eating Sound
리트리버를 소녀로 착각한 행성이 🐶 리트리버를 쫒아다녀요 🐕 신나는 제주도 바닷가 산책
아주아주 흉폭한 강아지
야외 노천탕 ♨ 즐기는 강아지 🕶 맨또롱더독 제주도 일상 🌴
소형견 눈치보는 대형견 🐶 사료 빌런 소녀와 용맹한 행성이 ㅋㅋㅋㅋ
제주도 생활이 행복한 강아지 소녀와 행성이 🌴 힐링 생활여행기 맨또롱더독 !
Pigs feet 🐷 mukbang Real Eating Sound 🌴 In Jeju Island Beautiful Healing with bird calls
강아지가 싫다던 아빠집에가니 생기는일 🐶 멘또롱더독 🌸 제주도 가는길
제발 장난감 던져달라고 울부짖는 강아지 ㅋㅋㅋ 소녀야 그렇게 장난감이 좋아?
강아지와 함께 제주도 한달반살이 🌸 멘또롱더독 티저영상 🐥
ENG SUB _ Hangseong's First Swim~ Let's Spend a Day at the Pool Pomeranian & Retriever
베이컨랜드에간 소행성 🐶 베이컨박스 리뷰
ENG SUB _ What Happens When a Large dog Can't Go For a Walk
ENG SUB _ Childhood of Baby Hangseong (It's Not Cotton Candy)
ENG SUB _ ​A Confident Superior Dog, Hangseong
ENG SUB _ Smart Dog with a Snack Dispenser
ENG SUB _ Dogs Coveting Each Other's Snacks ​
 닭발 아닌 오리발 리얼사운드  폭풍흡입하고 오리발 내미는 소녀
ENG SUB _ Dog Video It's Unfair~ Sonyeo, I'm the One Who Raised and Fed You
ENG SUB _ ​Sick Sonyeo, Playful Hangseong Dog Pet Video
ENG SUB _ I Blew into Her Ear and She's Whining to Stop Dog Pet Video
중성화 수술 했어요 🐶
강아지 빼빼로 개껌 리얼사운드
Retriever Eating with hands LOL Funny & Adorable Animal Video
움직이는 지네 장난감을 본 강아지의 반응은? 🐕
강아지들에게 TV를 보여줬어요 🌸 소녀와 행성이의 반응은?
july0325:~/workspace (master) $ ruby telegram.rb
telegram.rb:51:in `<main>': undefined local variable or method `i' for main:Object (NameError)
july0325:~/workspace (master) $ ruby telegram.rb
july0325:~/workspace (master) $ ruby telegram.rb
july0325:~/workspace (master) $ ruby telegram.rb
july0325:~/workspace (master) $ ruby telegram.rb
july0325:~/workspace (master) $ ruby telegram.rb
july0325:~/workspace (master) $ ruby telegram.rb
july0325:~/workspace (master) $ ruby telegram.rb
telegram.rb:96: syntax error, unexpected end-of-input, expecting keyword_end
july0325:~/workspace (master) $ ruby telegram.rb
july0325:~/workspace (master) $ ruby telegram.rb
july0325:~/workspace (master) $ ruby telegram.rb
july0325:~/workspace (master) $ ruby telegram.rb
july0325:~/workspace (master) $ 
```



