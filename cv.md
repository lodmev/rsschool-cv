# Dmitriy Lovyagin
### Junior Frontend Developer
## Contact information:
* E-mail: lodmev@gmail.com
* Telegram: [@lodmev](https://t.me/lodmev)
* [github.com](https://github.com/lodmev/)
## Briefly about me:
Currently work in car rapeir shop. I devote most of my free time to programming. 
I have written several programs and scripts, that help me and my colleagues in work. 
I like to study and learn something new about many things. 
## Skills:
* Git
* Linux
* Python
* Java Script
* Golang
## Completed courses:
* [Code Basics](https://code-basics.com):
   * HTML
   * CSS
* [Yandex Practicum](https://practicum.yandex.ru/):
    * Git Basics
## Code examples:
```JavaScript
const renderCalendar = () => {
  let firstDayOfMonth = new Date(currYear, currMonth, 1).getDay(), // getting first day of month
    lastDateOfMonth = new Date(currYear, currMonth + 1, 0).getDate(), // getting last date of month
    lastDayOfMonth = new Date(currYear, currMonth, lastDateOfMonth).getDay(), // getting last day of month
    lastDateOfLastMonth = new Date(currYear, currMonth, 0).getDate(); // getting last date of previous month
  let liTag = "";

  for (let i = firstDayOfMonth; i > 1; i--) {
    // creating li of previous month last days
    liTag += `<li class="inactive">${lastDateOfLastMonth - i + 1}</li>`;
  }

  for (let i = 1; i <= lastDateOfMonth; i++) {
    // creating li of all days of current month
    // adding active class to li if the current day, month, and year matched
    let isToday =
      i === date.getDate() &&
      currMonth === new Date().getMonth() &&
      currYear === new Date().getFullYear()
        ? "active"
        : "";
    liTag += `<li class="${isToday}">${i}</li>`;
  }

  for (let i = lastDayOfMonth; i < 7; i++) {
    // creating li of next month first days
    liTag += `<li class="inactive">${i - lastDayOfMonth + 1}</li>`;
  }
  currentDate.innerText = `${months[currMonth]} ${currYear}`; // passing current mon and yr as currentDate text
  daysTag.innerHTML = liTag;
};
```
