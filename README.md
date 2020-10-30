#include <iostream>
using namespace std;
#define N_UNIT    100 //N_UNIT  100으로 정의
#define ATTACK_UNIT   1 공격 유닛  1로 정의
#define PROTECT_UNIT  2 방어 유닛  2로 정의
class GameUnit //클래스 GameUnit, 가상함수로 Display와 DoAction을 정의하고 순수가상함수로 함.
{
public:
	virtual void Display(int x, int y) = 0;
	virtual void DoAction() = 0;
};
  
class AttackUnit : public GameUnit //GameUnit에 상속, AttackUnit Display와 DoAction 오버라이딩,
{
public:
	void Display(int x, int y) {}
	void DoAction() {}
};

class ProtectUnit : public GameUnit //GameUnit에 상속, ProtectUnit Display와 DoAction 오버라이딩,
{
{
public:
	void Display(int x, int y) {}
	void DoAction() {}
};

//출처 https://github.com/CppKorea/DesignPattern/blob/2020/master/Singleton/Singleton/Singleton2.cpp
