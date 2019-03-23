# demo-mode-summary
一、设计模式总结
简单工厂模式：需要什么工厂就创建什么
工厂方法模式：需要什么由具体的工厂来创建
抽象工厂模式：需要什么由具体的品牌工厂来创建
单例模式：任何情况人都只存在一个
代理模式：专业的事情找专业的人做
原型模式：身外化身
委托模式：将任务分发给专业的人士；
策略模式：行为不同，结果相同，条条大路通罗马；
模板方法模式：按照计划来执行，计划具体实现可变
适配器模式：将输入对象以需要的形式输出
装饰器模式：同宗同源，在原有的基础上增加新的东西；
观察者模式：有事通知我

二、SpringAOP、IOC、DI应用的代码片段

AOP：面向切面编程
<context:annotation-config/>
<context:component-scan base-package="com.tlf.*"/>

IOC：将类的控制权转移
<bean id="dwrBean" class="com.tlf.dwr.DwrBean">
		<property name="sessionFactory" ref="sessionFactory" />
</bean>

Dl：给类的属性赋值
public class UserInfo{
  // Fields
	private String userNo;
	private String name;

  public String getUserNo() {
		return this.userNo;
	}
	
	public void setUserNo(String userNo) {
		this.userNo = userNo;
	}
	
	public String getName() {
		return this.name;
	}
}
