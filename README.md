# Java_note

## 1  Objects.equals(Object a, Object b)方法
    public static boolean equals(Object a, Object b) {
        return (a == b) || (a != null && a.equals(b));
    }
