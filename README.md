# doudizhu
[onestraw](https://github.com/onestraw)/[doudizhu](https://github.com/onestraw/doudizhu) 项目的C++版本
## 示例
```c++
FTL ftl;
//"4-4-4-4-5-5-6-6"必须按照扑克牌大小，{"3","4","6","5","7"}不用
std::cout<<ftl.check(std::vector<std::string>{"3","4","6","5","7"})<<" "<<ftl.check("K-A-2-2-2")<<std::endl;
std::cout<<ftl.check("4-4-4-4-5-5-6-6","3-3-3-3","four_two_pair")<<std::endl;
std::cout<<ftl.type("4-4-4-4-5-5-6-6")[0].first<<" "<<ftl.type("4-4-4-4-5-5-6-6")[0].second<<std::endl;
std::cout<<ftl.type("5-5-6-6-7-7-7-7")[0].first<<" "<<ftl.type("5-5-6-6-7-7-7-7")[0].second<<std::endl;
std::cout<<ftl.type("3-4-5-6-7-8-9-10")[0].first<<" "<<ftl.type("3-4-5-6-7-8-9-10")[0].second<<std::endl;
```
### 输出
```
1 0
1
four_two_pair 2
four_two_pair 5
solo_chain_8 1
```
