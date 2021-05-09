``` c++
vector<int> setNumber(N,-1);

void union(int a, int b){
	int setNoA = setNumber[a];
	for(int i =0; i<N;++i){
		if(setNumber[i] == setNoA){
			setNumber[i] = setNumber[b];
		}
	}
}

bool find(int a, int b){
	if(setNumber[a] == setNumber[b]){
		return true;
	}
	return false;
}
```