# Java_note

## 1、Objects.equals(Object a, Object b)方法
    public static boolean equals(Object a, Object b) {
        return (a == b) || (a != null && a.equals(b));
    }
## 2、自动装箱和自动拆箱
    ArrayList<Integer> list = new ArrayList<>();
    list.add(3);//自动装箱，变换为list.add(Integer.valueOf(3));
    int n = list.get(0);//自动拆箱，变换为int n = list.get(0).intValue();
-128~127的short和int被包装到固定的对象之中
    Integer a = 127, b = 127, c = 128, d = 128;
    System.out.println((a==b)+" "+(c==d));//true false
