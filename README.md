int main()
{
	int sumpol = 0, protr = 1;
	int i, j;
	int x[3][4];
	for (int i = 0; i < 3; i++)
		for (int j = 0; j < 4; j++)
			scanf_s("%d", &x[i][j]);
	for (i = 0; i < 3; i++)
		for (j = 0; j < 4; j++)
		{
			if (x[i][j] > 0)
				sumpol += x[i][j];
			else
				protr *= x[i][j];
		}
	printf("%d, %d", sumpol, protr);
	return 0;
}
