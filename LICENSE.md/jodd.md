package jodd;

import jodd.http.HttpRequest;
import jodd.http.HttpResponse;
import jodd.mail.Email;
import jodd.mail.SendMailSession;
import jodd.mail.SmtpServer;
import jodd.util.StringPool;
import jodd.util.StringUtil;
import jodd.util.SystemUtil;

import static jodd.mail.CommonEmail.PRIORITY_HIGHEST;

/**
 *
 * Created by Cage on 2017/7/18 0018.
 *
 */
public class JoddCoreTest {


    public static void main(String[] args) {
        //jodd下的until下的StringUntil包下类的测试
        //String string1="abcdefg";
        //String string2="cg";
        //String string3="12";
        //System.out.println(string3.trim().length());
        //测试StringUntil下的方法remove
        //System.out.println(StringUtil.remove(string1,string2));//结果cdefg
        //测试StringUntil下的方法equals方法    String string2=new String("abcdefg");//true
        //如果其中一个参数为null是否会抛出异常   无论哪个参数为null都不会抛出异常       如果两者都为null则为true    null;
        //String string4=null;
        ///System.out.println(StringUtil.equals(string1,string4)); //false
        //使用isEmpty时如果字符串是 String string3="   "这种的就是false也就意味这判断为这个字符串不是空
        //isEmpty只能判断字符串是否为null和该字符串的长度是否为0
        //但是如果isBlank时则为true     在判断一个字符串是否为空的时候应当用isBlank
        //System.out.println(StringUtil.isBlank(string3));
        //字符串替换的方法
        //System.out.println(StringUtil.replace(string1,string2,string3));
        //char [] chars=new char[]{'c','g'};
        //char [] chars1=new char[]{'1','2'};
        //两个char数组的长度必须相同
       // System.out.println(StringUtil.replaceChars(string1,chars,chars1));
        //System.out.println()快捷键sout
        //System.out.println(SystemUtil.javaVersionNumber());   //输出当前工作目录

        /**
         * 测试jodd Http包下的
         */
        //httpRequest.send();
        //HttpResponse httpResponse=HttpRequest.get("https://lib.fxbtg-bank.com/regist/custom").send();
        //HttpRequest hr=new HttpRequest();
        //hr.queryEncoding(StringPool.UTF_8);
        //hr.get("https://lib.fxbtg-bank.com/regist/custom").send();
        //hr.get("https://lib.fxbtg-bank.com/regist/custom").send().body()
        //HttpRequest.get("https://signalmust.com").send().charset("UTF-8").body()
        /*System.out.println(HttpRequest.post("https://signalmust.com/main.html")
                .query("username","13373932106")
                .query("password","123456").send());*/
        //System.out.println("");


        /*String ll=StringUtil.split(HttpRequest.get("https://lib.fxbtg-bank.com/regist/custom").send().bodyText()
                                    ,",")[StringUtil.split(HttpRequest.get("https://lib.fxbtg-bank.com/regist/custom").send().bodyText()
                ,",").length-1];

        String message=StringUtil.removeChars(
                HttpRequest.get("https://lib.fxbtg-bank.com/regist/custom").send().bodyText(),
                '}','"');
        String result=StringUtil.split(message,":")[StringUtil.split(message,":").length-1];
        System.out.println(result);*/
        /**
         * 使用 jodd中的 Email发送
         */
        /*Email email=Email.create()
                         .from("发送的账户")
                         .to("接受的账户")
                         .subject("测试呀")
                         .addText("啦啦啦啦啦啦啦");
        SendMailSession session =null;
        try {
            //写服务器验证
            SmtpServer smtpServer = SmtpServer.create("邮箱的服务器地址")
                                              .authenticateWith("发送账户名", "密码");
            session = smtpServer.createSession();
            session.open();
            session.sendMail(email);
            session.close();
        }catch (Exception e){
            e.printStackTrace();
            System.out.println("出错了！");
        }finally {
            //关闭服务
            if( null !=session){
                session.close();
            }
        }*/























    }



}
