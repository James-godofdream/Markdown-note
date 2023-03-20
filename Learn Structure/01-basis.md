# Preview knowledge
***
## C++ 模板
#### template\<class T>
#### class Table{
    public:
    T a;
    T b;
};
#### int main{
    Table<int> t;
    t.a = 3;
    t.b = 4;
    Table<double> tt;
    tt.c = 3.1;
    tt.d = 4.2;
};
### <<代码重构
#### class Stu{
    private:
        string id;
        string score;
    public:
        Stu(string id,int score){
            this->id = id;
            this->score = score;
        }
    friend ostream& operator << (ostream& o,const Stu& s);
}
#### ostream& operator << (ostream& o,const Stu& s){
    o<<"("<<s.id<<","<<s.score<<")";
    return 0;
}
### vector用法
#### `vector<int> v;`
#### `v.push_back(123);`
#### `v.empalce_back("s001",98);`
### vector依次输出
#### {
    for(auto x:v)
        cout<<x<<end1;
}
## Java 泛型（generic type)
### class Table\<T>{
    public int a;
    public int b;
}
#### 使用需要指定类型，不能直接创建实例
#### {
    Table<integer> t = new Table<>();
    t.a = 3;
    t.b = 4;
    Table<Double> tt = new Table<>();
    tt.a = 5.2;
}
#### 注意：尖括号中不能使用原始类型
### Java中的顺序表ArrayList的引入与声明
#### `import java.util.ArrayList;`
#### {
    ArrayList<Stu> al = new ArrayList<>();
    Stu zs = new Stu();
    zs.id = "S001";
    Stu ls = new Stu();
    ls.id = "S002";
    al.add(zs);
    ls.add(ls);
    System.out.println(al);
}

### 重写toString()以便显示结果
#### class Stu{
    public String id;
    public String score;
    publec String toString(){
        return "("+id+","+name+")";
    }
} 
## Python 不需要泛型/模板
### C/C++中sizeof()不是函数,是个运算符
