# java-11.09
## 计G201 2020322079 尚万帅
## 1. 实验内容
+ 1.设计两个管理接口：学生管理接口和教师管理接口。学生接口必须包括缴纳学费、查学费的方法；教师接口包括发放薪水和查询薪水的方法。

+ 2.设计博士研究生类，实现上述的两个接口，该博士研究生应具有姓名、性别、年龄、每学期学费、每月薪水等属性。    

+ 3.编写测试类，并实例化至少两名博士研究生，统计他们的年收入和学费。根据两者之差，算出每名博士研究生的年应纳税金额。
## 2. 实验设计

+ 1.设置Colleagestudent
```
   public static void payment() {   //接口中的方法都是静态的方法  
 

 }
 public static void checkmany() { //学生类中的查询学费的方法
 
 }
```
+ 2. Teacher 接口中的方法

```
 public static void paysalary() {
 
  }
  public static void inquiresalary() {
 
  }
```
 ## 3. 核心方法
 
 1. Doctoral类实现接口中的博士生的缴费功能和获取缴费成功的信息的方法。
  
  ```
     public void payment() {
		Doctoral Doctoral2 = new Doctoral();
		SchoolFinance  scw=new SchoolFinance();
		String str="输入你要交的学费";
		scw.setMoney(20000);
		while(true) {
			System.out.println(str);
			Scanner sc=new Scanner(System.in);
			int id1;
			int b=scw.getMoney();
    	try {
    		id1=sc.nextInt();
    		if(id1==b) {
    			System.out.println("你的学费支付了："+id1+"元,支付成功");
         		break;
    		}else {
    			 System.out.println("你输入的有误");
    			 
    		}
     		
		} catch (Exception e) {
			str="您输入有误,请输入一个整数:";
			continue;
		} 	
     }
		
	}
  ```
  + 2.检查博士生缴费的钱数
 public void checkmany() {
  try {
   sv.setMoney(10000);
   d=sv.getMoney();
  } catch (Exception e) {
   System.out.println("你输入的不正确");
  }
  
  System.out.println("您查询的学费为"+d);
 }
 public void paysalary() {
  System.out.println("每个月发放的薪水为："+doctoral);
 }
  
  ```
  2. 调用博士类并且通过Scanner类进行输出姓名，性别，年龄，和缴费中的方法。
      ```
        Scanner sc=new Scanner(System.in);
      System.out.println("请输入姓名");
     name=sc.nextLine();
     System.out.println("请输入性别");
      String sex=sc.next();
      System.out.println("请输入年龄");
      int age=sc.nextInt();
      System.out.println("姓名："+name);
      System.out.println("性别："+sex);
      System.out.println("年龄："+age);
 }
       ```
   
  ## 4.实验截图
  
https://github.com/1141565458sws/java-11.09/blob/main/swssss/sws.png

  ## 5.实验感想

  1. 通过这个实验学习到了如何设计管理接口。
  2. 学会了如何输出博士生的类的相关需求。
  3. 学会了如何捕获异常。
