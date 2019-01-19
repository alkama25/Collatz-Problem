# Collatz-Problem
int main() {
  //According to the question the length of the sequence is given as 1 million.
  unsigned N = 1000000;
  //Now we will create three type of arrays. The first array will denote the length, the second array will point to the next element in the sequence and the third one will denote the status of the current element pointed.
  unsigned length[ N + 1]={ 0 };
  unsigned next [N + 1]={ 0 };
  unsigned status [N + 1]={ 0 };
  
  //Now we will initialize the declared arrays.
  for (unsigned i = 1; i <= N; i++) {
		length[i] = 1; //Here the initial length is 1.
		next[i] = i; 
		status[i] = 0; //The initial status is zero.
	}
  
  // Set the status of no i=1 to done
	status[1] = 1;
