# 今天带来的是娱乐代码

### QQ聊天轰炸机





1. ## 首先咱们来看代码

   ```python
   import time
   import random
   from pynput.keyboard import Controller as key_col
   from pynput.mouse import Button,Controller
   # 以上是需要安装的模块，下面我会介绍。
   
   print('开始消息轰炸',time.sleep(3))# 开始时候延迟秒数，别太短，怕你反应不过来。
   
   li = '新人求关注','我爱python','我爱博客园'# 随机内容，按照我的格式可以无限增加
   
   def keyboard_input(string):
       keyboard = key_col() #控制键盘
       keyboard.type(string) #键盘输入string
   def mouse_click():
       mouse = Controller() # 控制鼠标
       mouse.press(Button.left) # 按住鼠标左键
       mouse.release(Button.left) # 松开鼠标左键
   def main(number,string):
       time.sleep(0.1) # 每个消息间隔秒数，不要太小，怕电脑爆炸
       for i in range(number):
           keyboard_input(string)
           mouse_click()
           time.sleep(0.1)# 每个消息间隔秒数，不要太小，怕电脑爆炸
   count = 0
   while count < 100:# 这里面100就是随机次数，友情提示不要太大。
       if __name__ == '__main__':
           main(1,f'{random.sample(li,1)}')
           count += 1
   print('轰炸结束')
   ```

2. #### 效果上面就是按照你输的随机内容轰炸100次，当然都是可以改动，建议次数不要太大，间隔不要太小，不然电脑死机不要怪我哈哈哈。

3. #### 操作方法：

   1. 首先打开你需要轰炸的人的聊天界面。
   2. 然后点一下内容栏，然后快把鼠标放在发送按钮上，一定要放在上面！！！！
   3. 然后就会开始轰炸，轰炸期间不要动鼠标，不然就会到处乱按和打字。
   4. 如果对自己速度没有信心，就把开始延迟调大一点就行了。

4. 建议使用时候开启微软自带输入法，不然可能打出来的子不一样，另外输入随机内容时候建议也使用微软自带输入法，输入法也有记忆，敲了一次不容易出错。





2. ## 接下来的非常关键，出错可能都在接下来的上面

   1. 导入模块：

      1. 忘记说了一个重要点了，一切的前提你要安装python
      2. 打开cmd输入：
         1. pip install pywin32
         2. pip insatll pynput
      3. 其实只需要导入一个就行了，我忘记了，我好不称职啊^_^。
      4. 在文本文档中粘贴代码，保存退出，将后缀名改为py
      5. 然后点击文件就开始运行了，然后就是我上面的操作了

      

      

      

3. ## 操作都完成了，这是我亲自实验的过程，当然可能都有些问题，毕竟涉及到了导入模块。

   1. 遇到问题可以自行进行百度，有很多大佬博客会有解决方法。
   2. 如果无法解决，就下方留言吧，我会尽力解决的。



