### gotcha 👋
```
#include <iostream>
#include <time.h>

int getGrade(int data[])
{
	int sum = 0;
	int num = rand() % 100;

	for (int i = 0; i < 5; i++)
	{
		sum += data[i];

		if (num < sum)
		{
			return i + 1;
		}
		std::cout << sum << std::endl;
	}
}

int main()
{
	srand(time(NULL));

	int result = 0;
	int grade[5] = { 0, };
	int data1[5] = { 50,30,10,7,3 };
	int data2[5] = { 30,20,10,5,5 };

	int a = 0;
	std::cin >> a;

	for (int i = 0; i < a; i++)
	{
		result = getGrade(data1);

		grade[result - 1]++;
	}
	
	for (int i = 0; i < 5; i++)
	{
		std::cout << i + 1 << "성: " << grade[i] << std::endl;
	}

	return 0;
}
```
<!--
**kimseong07/kimseong07** is a ✨ _special_ ✨ repository because its `README.md` (this file) appears on your GitHub profile.

Here are some ideas to get you started:

- 🔭 I’m currently working on ...
- 🌱 I’m currently learning ...
- 👯 I’m looking to collaborate on ...
- 🤔 I’m looking for help with ...
- 💬 Ask me about ...
- 📫 How to reach me: ...
- 😄 Pronouns: ...
- ⚡ Fun fact: ...
-->
