int silnia(int a){
	if(a == 0)	return 1;
	int n = a;	
	if(a < 0)	return 0;
	else		return n *= silnia(n-1);
}

int main(){
	int a, b;
	scanf("%d %d", &a, &b);
	if((a > 0) && (b > 0) && (a > b))
		printf("%d\n", silnia(a)/(silnia(b)*silnia(a-b)));
	else
		printf("Podane bledne dane\n");
	//printf("%d %d", silnia(a), silnia(b));
	return 0;
}
