- to_string()
- unordered_map<,>
	- find()
	- []
- sort(vector.begin(), vector.end())
  - sort( values.begin( ), values.end( ), [ ]( string a,string b )
    {
      return a < b;
    });
- char to string coversion
  - string s(1, ch.first)
- std::unique
  - removing duplicates from array
- std::erase
  - deleting element(s) while traversion
- how to create min_heap
  - ```
    priority_queue<long long,vector<long long>,greater<long long> > q;
        q.push(0);
        q.top();
        q.pop();
    ```
  - ```
    priority_queue<pair<int,int>, vector<pair<int,int>>,  std::function<bool(const pair<int,int>& a, const pair<int,int> &b)>> candidates(
            [](const pair<int,int>& a, const pair<int,int> &b){
            return a.first > b.first;
        });
    ```
- how to have custom comparator for sort
- [dequeue](https://www.cplusplus.com/reference/deque/deque/)
- accumulate(vec.begin(), vec.end(), 0)
- nth_element https://www.geeksforgeeks.org/stdnth_element-in-cpp/
- 