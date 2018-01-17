# common_elReg
# 校验基本日期格式
var reg1 = /^\d{4}(\-|\/|\.)\d{1,2}\1\d{1,2}$/;
var reg2 = /^(^(\d{4}|\d{2})(\-|\/|\.)\d{1,2}\3\d{1,2}$)|(^\d{4}年\d{1,2}月\d{1,2}日$)$/;
# 校验密码强度
var reg = /^(?=.*\\d)(?=.*[a-z])(?=.*[A-Z]).{8,10}$/;
# 校验中文
var reg = /^[\\u4e00-\\u9fa5]{0,}$/;
# 由数字、26个英文字母或下划线组成的字符串
var reg = /^\\w+$/;
# 校验E-Mail 地址
var reg = /[\\w!#$%&'*+/=?^_`{|}~-]+(?:\\.[\\w!#$%&'*+/=?^_`{|}~-]+)*@(?:[\\w](?:[\\w-]*[\\w])?\\.)+[\\w](?:[\\w-]*[\\w])?/;
# 校验身份证号码
  # 15位:
    var reg = /^[1-9]\\d{7}((0\\d)|(1[0-2]))(([0|1|2]\\d)|3[0-1])\\d{3}$/;
  # 16位:
    var reg = /^[1-9]\\d{5}[1-9]\\d{3}((0\\d)|(1[0-2]))(([0|1|2]\\d)|3[0-1])\\d{3}([0-9]|X)$/;
# 校验日期
 # "yyyy-MM-dd" 格式的日期校验，已考虑平闰年。
var reg = /^(?:(?!0000)[0-9]{4}-(?:(?:0[1-9]|1[0-2])-(?:0[1-9]|1[0-9]|2[0-8])|(?:0[13-9]|1[0-2])-(?:29|30)|(?:0[13578]|1[02])-31)|(?:[0-9]{2}(?:0[48]|[2468][048]|[13579][26])|(?:0[48]|[2468][048]|[13579][26])00)-02-29)$/;
# 校验金额
var reg = /^[0-9]+(.[0-9]{2})?$/;
# 校验手机号
 # 下面是国内 13、15、18开头的手机号正则表达式。（可根据目前国内收集号扩展前两位开头号码）
var reg = /^(13[0-9]|14[5|7]|15[0|1|2|3|5|6|7|8|9]|18[0|1|2|3|5|6|7|8|9])\\d{8}$/;
