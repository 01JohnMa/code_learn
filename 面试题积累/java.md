1、深拷贝与浅拷贝的区别
使用浅拷贝在拷贝对象的时候会复制对象本身以及基本类型成员变量，如果包含引用类型的成员变量则智慧复制其地址值
```java
  public  class  Person implement Cloneable{
  int age ;
  String name;
  Street street;
  @override 
    public Obeject  clone throws CloneNotSupportedException {
    //浅拷贝
      return  super.clone();
    }
  public class Address{
    private address
  }
  }
  public  class  Person implement Cloneable{
  int age ;
  String name;
  Street street;
  @override 
    public Obeject  clone throws CloneNotSupportedException {
    //深拷贝
      Person cloned = (Person) super.clone();
     cloned.adress = new Adress(this.address.getAdress());
     return  cloned;
    }
  public class Address implement{
    private String  address
    Adress(adress){
      this.adress = adress;
    }
    @Override
    protected Object clone() throws CloneNotSupportedException {
        return super.clone();
    
  }
  }
```
2、集合 map set list那些
3、循环依赖怎么解决
