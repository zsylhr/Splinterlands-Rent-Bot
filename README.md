# Splinterlands-Rent-Bot
A bot can help you rent Splinterlands cards in PeakMonsters

Download from the release

explain:

4 functions, through setting settings.txt file
Function 0 and 2 doesn't need gas
Function 1 : 1+power/3000 dec
Function 3 : 2 dec

Function: 0 --- authorize an account to rent a card to peakmonster. Each account can only be authorized once. If it has been authorized on the website before, it does not need to be re authorized

Function: 1 --- set the bid of the leased card. The parameters are the upper and lower range of power, the value of bid (how many power cards a Dec rents), the minimum power of each leased card, and the multi-threaded mode. It is recommended not to exceed 3

Function: 2 --- cancel the bid and invalidate the bid you set

Function: 3 --- cancel rental card. PK website rents a card for two days. If there is a card for two days, this function will automatically return it for one day

Note: only function: 1 needs to set the bid parameter, and other functions only need to set the number of threads

Account: user.txt, separated by English commas,

Such as aaa,bbb,ccc,ddd
Or:
aaa,
bbb,
ccc,
ddd


Password: posting_Key and active_Key, the two passwords of each account should be put in password.txt file and cannot be repeated. The format is the same as user.txt same
posting_Key and active_Key can be placed at random and can be arranged at will, as long as the middle is separated by English commas

post1,
post2,
active3,
post3,
active1,
active2

This bot will charge some gas which depends on the power you want to rent.

说明：
4种功能，通过设置settings.txt文件中function的值来进行选择
function:0   ---  授权账户给PeakMonster租卡，每个账户只用授权一次，如果之前已经在网站上进行过授权，不需要再授权
function:1   ---  设置租卡的bid, 参数分别是power的上下范围，BID的值(一个dec租多少power的卡)，租的每张卡的最低power, 多线程模式，建议设置不要超过3
function:2   ---  取消bid，使你设置的bid失效
function:3   ---  退租卡片，pk网站租卡是两天的，如果有两天卡，使用此功能会自动退一天

function 0 和 1 不收取手续费
function 1 手续费为 1+power/3000 dec
function 3 手续费为 2 dec

注：只有function:1才需要设置bid的参数，其余功能只用设置线程数

账户：user.txt中存放用户名，以英文逗号隔开，
如： aaa,bbb,ccc,ddd
或者：
aaa,
bbb,
ccc,
ddd

密码：password.txt中存放posting_key与active_key，每个账户的两个密码都要放在此文件中，且不能重复，格式与user.txt相同
posting_key与active_key位置随意，可任意排放，只要中间以英文逗号隔开即可

post1,
post2,
active3,
post3,
active1,
active2

脚本会收取一些手续费，手续费的数量与你租卡的power值有关，但与你的租金相比会很少
