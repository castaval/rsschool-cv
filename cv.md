# Alexander Butusov

## Contact

### Mail 
alexander.kiosk@gmail.com

### Telegram
@Algrimbut

### Discord
Kiosk#2370

## About Me
My goal is to become a developer who can work both Front-End and Back-End. 

My priorities are self-development and self-realization.

My strengths are that I am willing to accept my mistakes and work on them.

I have no work experience, but I am always ready to learn about new things.

### Skills
1. C++
2. Python 
3. Django
4. Git

### Code Example
#### C++
```C++
#include <vector>

std::vector<int> countPositivesSumNegatives(std::vector<int> input)
{
  int count = 0;
  int sum = 0;
  for(int i = 0; i < input.size(); i++){
    if(input[i] > 0){
      count++;
    }
    if(input[i] < 0){
      sum += input[i];    
    }
  }
  std::vector <int> CountSum = {count, sum};
  if(count != 0 || sum != 0){
    return CountSum;
  } else {
      return {};
  }
} 
```
#### Python
``` Python
async def stop(message: types.Message, state: FSMContext):
    goals = await sqlite_db.sql_goals_read()
    if goals is None:
        async with state.proxy() as data:
            message_goal = """{}
{} """.format(list(data.values())[0], 'Список пуст')
        await bot.send_message(message.from_user.id, message_goal, reply_markup=get_inline_keyboard())
    else:
        all_goals = ()
        for goal in goals:
            all_goals += goal
        async with state.proxy() as data:
            message_goal = """{}
{}""".format(list(data.values())[0], '\n'.join(all_goals))
        await bot.send_message(message.from_user.id, message_goal, reply_markup=get_inline_keyboard())
    await InlineFSM.new_goal.set()
```
### Experience
I created a [TODO-bot](https://github.com/castaval/telegram-todo-bot.git) on Python 
