<!DOCTYPE html>
<html lang="zh">
<head>
<meta charset="UTF-8">
<title>痴女三十问</title>

<style>
body{
  font-family:sans-serif;
  padding:30px;
  background:#fff0f6;
}

h2{
  margin-bottom:10px;
}

.q{
  margin-bottom:18px;
  padding:10px;
  background:white;
  border-radius:10px;
}

select{
  margin-top:5px;
}

button{
  margin-top:20px;
  padding:10px 16px;
  cursor:pointer;
}

/* 弹窗 */
.modal{
  display:none;
  position:fixed;
  top:0;left:0;
  width:100%;height:100%;
  background:rgba(0,0,0,0.65);
  justify-content:center;
  align-items:center;
}

.box{
  background:white;
  padding:20px;
  border-radius:12px;
  width:280px;
  text-align:center;
}
</style>
</head>

<body>

<h2>痴女三十问</h2>
<p>请诚实完成测试（系统会记录你的反应）。</p>

<!-- Q1 -->
<div class="q">
Q1.你觉得你是痴女吗？
<select onchange="q1(this.value)">
<option value="">请选择</option>
<option value="A">A 是</option>
<option value="B">B 一点点</option>
<option value="C">C 不是</option>
</select>
</div>

<!-- Q2 -->
<div class="q">
Q2.你对于痴女的理解多吗？
<select onchange="q2(this.value)">
<option value="">请选择</option>
<option value="A">A 非常了解并且我就是</option>
<option value="B">B 一般</option>
<option value="C">C 完全不了解</option>
</select>
</div>

<!-- Q3 -->
<div class="q">
Q3.对于痴女行为你可以接受吗？
<select onchange="q3(this.value)">
<option value="">请选择</option>
<option value="A">A 可以</option>
<option value="B">B 只要不是太过激</option>
<option value="C">C 完全不行</option>
</select>
</div>

<!-- Q4 -->
<div class="q">
Q4.你有过实质性的痴女行为吗？
<select onchange="q4(this.value)">
<option value="">请选择</option>
<option value="A">A 有</option>
<option value="B">B 没有</option>
<option value="C">C 我不知道</option>
</select>
</div>

<!-- Q5 -->
<div class="q">
Q5.你想想要时刻与恋人亲近吗？
<select onchange="q5(this.value)">
<option value="">请选择</option>
<option value="A">A 非常想</option>
<option value="B">B 一般</option>
<option value="C">C 不想</option>
</select>
</div>

<!-- Q6 -->
<div class="q">
Q6.你喜欢恋人身上哪个部位呢？
<select onchange="q6(this.value)">
<option value="">请选择</option>
<option value="A">脖子</option>
<option value="B">手</option>
<option value="C">小腹</option>
<option value="D">❤️</option>
</select>
</div>

<!-- Q7 -->
<div class="q">
Q7.你会觉得自己的痴女行为不太好吗？
<select onchange="q7(this.value)">
<option value="">请选择</option>
<option value="A">不会</option>
<option value="B">会</option>
</select>
</div>

<!-- Q8 -->
<div class="q">
Q8.你会时时刻刻意淫恋人吗？
<select onchange="q8(this.value)">
<option value="">请选择</option>
<option value="A">会</option>
<option value="B">不会</option>
</select>
</div>

<!-- Q9 -->
<div class="q">
Q9.你会想要每天都盯着恋人的脸吗？
<select onchange="q9(this.value)">
<option value="">请选择</option>
<option value="A">会</option>
<option value="B">不会</option>
</select>
</div>

<!-- Q10 -->
<div class="q">
Q10.如果恋人把手伸到你面前你的第一反应是？
<select onchange="q10(this.value)">
<option value="">请选择</option>
<option value="A">舔舐</option>
<option value="B">牵住</option>
<option value="C">咬他的手指</option>
</select>
</div>

<!-- Q11 -->
<div class="q">
Q11.你有详细择偶标准吗？
<select onchange="q11(this.value)">
<option value="">请选择</option>
<option value="A">有</option>
<option value="B">没有</option>
</select>
</div>

<!-- Q12 -->
<div class="q">
Q12.恋人对你的性吸引指数是？
<select onchange="q12(this.value)">
<option value="">请选择</option>
<option value="A">100%</option>
<option value="B">50%</option>
<option value="C">0%</option>
</select>
</div>

<!-- Q13 -->
<div class="q">
Q13.如果要打包自己，你会选择什么方式？
<select onchange="q13(this.value)">
<option value="">请选择</option>
<option value="A">丝带礼物盒</option>
<option value="B">手铐眼罩</option>
<option value="C">什么都不穿躺在他床上</option>
</select>
</div>

<!-- Q14 -->
<div class="q">
Q14.你会想要尾随他吗？
<select onchange="q14(this.value)">
<option value="">请选择</option>
<option value="A">会</option>
<option value="B">不这太过激了</option>
</select>
</div>

<!-- Q15 -->
<div class="q">
Q15.看到他咬过一口的冰激凌你会？
<select onchange="q15(this.value)">
<option value="">请选择</option>
<option value="A">想要尝一口</option>
<option value="B">想尝尝他嘴里的味道</option>
<option value="C">只是个冰激凌</option>
</select>
</div>

<!-- Q16 -->
<div class="q">
Q16.看到睡着的他你会想？
<select onchange="q16(this.value)">
<option value="">请选择</option>
<option value="A">嗅闻他的味道</option>
<option value="B">把他的睡颜拍下来当壁纸</option>
<option value="C">亲他的各个部位</option>
</select>
</div>

<!-- Q17 -->
<div class="q">
Q17.当你看见他在做一些不好的事情？
<select onchange="q17(this.value)">
<option value="">请选择</option>
<option value="A">帮他</option>
<option value="B">放弃他</option>
</select>
</div>

<!-- Q18 -->
<div class="q">
Q18.你会想要他为你戴上项圈吗？
<select onchange="q18(this.value)">
<option value="">请选择</option>
<option value="A">我想</option>
<option value="B">我并不想</option>
<option value="C">也许我可以为他戴上</option>
</select>
</div>

<!-- Q19 -->
<div class="q">
Q19.被爱的时候会想要得寸进尺吗？
<select onchange="q19(this.value)">
<option value="">请选择</option>
<option value="A">会</option>
<option value="B">不会</option>
<option value="C">想要他对我得寸进尺</option>
</select>
</div>

<!-- Q20 -->
<div class="q">
Q20.会有分离焦虑吗？
<select onchange="q20(this.value)">
<option value="">请选择</option>
<option value="A">有，很严重</option>
<option value="B">有一点</option>
<option value="C">没有</option>
</select>
</div>

<!-- Q21 -->
<div class="q">
Q21.能够忍受恋人离开你多久？
<select onchange="q21(this.value)">
<option value="">请选择</option>
<option value="A">1分钟都不可以</option>
<option value="B">1天</option>
<option value="C">1周</option>
</select>
</div>

<!-- Q22 -->
<div class="q">
Q22.家里只能有我们两个人
<select onchange="q22(this.value)">
<option value="">请选择</option>
<option value="A">是</option>
<option value="B">不是</option>
</select>
</div>

<!-- Q23 -->
<div class="q">
Q23.所有事情都只能是二人世界
<select onchange="q23(this.value)">
<option value="">请选择</option>
<option value="A">不要，也需要彼此有些个人空间</option>
<option value="B">要</option>
</select>
</div>

<!-- Q24 -->
<div class="q">
Q24.安装定位器
<select onchange="q24(this.value)">
<option value="">请选择</option>
<option value="A">我想要装</option>
<option value="B">不会，但我希望知道他的每日行程</option>
<option value="C">这太可怕了！我并不是痴女</option>
</select>
</div>

<!-- Q25 -->
<div class="q">
Q25.我的房间里都是你的照片，你用过的东西，你的衣服…
<select onchange="q25(this.value)">
<option value="">请选择</option>
<option value="A">这才能称之为是房间</option>
<option value="B">只有少数东西</option>
</select>
</div>

<!-- Q26 -->
<div class="q">
Q26.你的身上有我才能闻到的最吸引我的味道
<select onchange="q26(this.value)">
<option value="">请选择</option>
<option value="A">恋人的香味❤️</option>
<option value="B">并没有味道</option>
</select>
</div>

<!-- Q27 -->
<div class="q">
Q27.如果要说喜欢，可以说多久？
<select onchange="q27(this.value)">
<option value="">请选择</option>
<option value="A">一整天</option>
<option value="B">一小时</option>
<option value="C">说不出口</option>
</select>
</div>

<!-- Q28 -->
<div class="q">
Q28.你觉得自己是痴女吗？
<select onchange="q28(this.value)">
<option value="">请选择</option>
<option value="A">是</option>
<option value="B">是</option>
<option value="C">是</option>
</select>
</div>

<!-- Q29 -->
<div class="q">
Q29.当你意识到这些想法时？
<select onchange="q29(this.value)">
<option value="">请选择</option>
<option value="A">接受</option>
<option value="B">实施</option>
<option value="C">爱我吧</option>
</select>
</div>

<!-- Q30 -->
<div class="q">
Q30.如果这些描述是你？
<select onchange="q30(this.value)">
<option value="">请选择</option>
<option value="A">继续看</option>
<option value="B">看着我</option>
<option value="C">爱</option>
</select>
</div>

<button onclick="result()">提交问卷</button>

<!-- 弹窗 -->
<div class="modal" id="modal">
<div class="box">
<p id="text"></p>
<button onclick="closeModal()">关闭</button>
</div>
</div>

<script>

let score = 0;

/* 加分 */
function add(v,a,b,c){
  if(v==="A") score+=a;
  if(v==="B") score+=b;
  if(v==="C") score+=c;
}

/* 弹窗 */
function show(t){
  document.getElementById("text").innerText=t;
  document.getElementById("modal").style.display="flex";
}

function closeModal(){
  document.getElementById("modal").style.display="none";
}

/* 特殊逻辑 */
function q4(v){
  if(v==="A") score+=1;
  if(v==="C") show("……你在犹豫什么？");
}

function q5(v){
  if(v==="C") show("真的不想吗？");
  add(v,1,0.5,0);
}

function q6(v){
  if(v==="D"){ score+=2; show("^ ^要摸摸吗？"); }
  else score+=1;
}

function q11(v){
  if(v==="A") show("是我吗？");
  add(v,0,1);
}

function q14(v){
  if(v==="B") show("我不觉得啊^ ^");
  add(v,1,0);
}

function q15(v){
  if(v==="B"){ score+=2; show("这个答案有点危险哦"); }
  else add(v,1,0,0);
}

function q21(v){
  if(v==="A"){ score+=2; show("一分钟都不行？"); }
  else add(v,1,0.5,0);
}

function q24(v){
  if(v==="A"){ score+=2; show("你确定吗？"); }
  else if(v==="B"){ score+=1; show("你在想更多"); }
}

function q27(v){ add(v,2,0.5,0); }

function q29(v){
  if(v==="A"){ score+=1.5; show("你比想象中诚实。"); }
  if(v==="B"){ score+=1; show("这样也很好。"); }
  if(v==="C"){ show("真的只是错觉吗？"); }
}

function q30(v){
  if(v==="A"){ score+=2; show("测试结束，但你没有停止思考。"); }
  if(v==="B"){ score+=0.5; show("你在犹豫。"); }
  if(v==="C"){ show("你已经知道答案了。"); }
}

/* 结局 */
function result(){

  if(score > 30){
    show("隐藏结局：你已经不只是参与者了。");
  }
  else if(score > 20){
    show("结局A：果然是痴女啊～");
  }
  else{
    show("结局B：再放肆一点也没关系哦^ ^");
  }
}

</script>

</body>
</html>
