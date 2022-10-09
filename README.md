# studyC
1-100顺序二分法


int main() {
	int a[100] = {0};
	int i, want, left = 0,right=99,k;
		for (i = 0; i < 100; i++) {
			a[i] = i + 1;
		

	}
	scanf("%d", &want);
	for (;left<=right;) {     //'<'is wrong
		k = (left + right)/2;
		if (a[k] ==want) {     //do not use '='
			break;
		}
		    else if (a[k] > want)
		{
			right = k - 1;
		}
		    else
		{
			left = k + 1;
		}
		printf("%d\n", k);
	}
	printf("=%d", a[k]);
	return 0;
}
