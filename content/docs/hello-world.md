---
id: hello-world
title: Hello World
permalink: docs/hello-world.html
prev: cdn-links.html
next: introducing-jsx.html
---

ខាងក្រោមនេះជាឧទាហរណ៍តូចមួយរបស់ React

```js
ReactDOM.render(
  <h1>Hello, world!</h1>,
  document.getElementById('root')
);
```

វាបង្ហាញពាក្យ "Hello, world!" ជាទំរង់ Heading នៅលើទំព័រ។

[](codepen://hello-world)

សូមចុចលើតំណភ្ជាប់ខាងលើសំរាប់បើកផ្ទាំងសរសេរកូដនៅលើបណ្តាញ។ លោកអ្នកអាចកែកូដតាមចិត្ត ដើម្បីឃើញលទ្ធផល។ ទំព័រភាគច្រើនក្នុងមគ្គុទេសក៍នេះនឹងមានឧទាហរណ៍ដែលលោកអ្នកអាចកែបាន ដូចមួយនេះអញ្ចឹង។


## របៀបអានណែនាំនេះ {#how-to-read-this-guide}

នៅក្នុងណែនាំ យើងនឹងពិនិត្យនិយាយពីប្លុកកូតរបស់ Reactគឺ៖ ធាតុ និង សមាសធាតុ។ នៅ​ពេល​អ្នក​ចេះ​ច្បាស់​ហើយ​​ អ្នកអាចបង្កើតកម្មវិធីដែល​ស្មុគស្មាញ​ពីបំណែកកូតតូចៗដែលអ្នកអាច​យកមកប្រើឡើងវិញបាន។


>គន្លឺះ
>
>ការណែនាំនេះត្រូវបានរចនាឡើងសម្រាប់មនុស្សដែលចូលចិត្ត **រៀនតាមដំណាក់កាល**. ប្រសិនបើអ្នកចូលចិត្តរៀនតាមរយៈការធ្វើ, សូមមើល [ការបង្រៀនជាក់ស្តែង](/tutorial/tutorial.html). អ្នកនឹងមើលឃើញថា ការណែនានេះ និង ការបង្រៀនមានទំនាក់ទំនងគ្នាទៅវិញទៅមក។

នេះជាជំពូកដំបូង​ដែលនិយាយអំពី ការណែនាំស្តីអំពីទ្រឹស្តីចម្បងរបស់ React។ លោកអ្នកអាចស្វែងរកតារាងមាតិកាទាំងអស់នៅផ្នែកខាងស្តាំ។ ប្រសិនបើអ្នកកំពុងប្រើឧបករណ៍ចល័តដើម្បីអាន អ្នកអាចស្វែងរកតារាងមាតិកាបាន​ដោយគ្រាន់តែចុច​ប៊ូតុងដែលស្ថិតនៅផ្នែកខាងក្រោមឈាងខាងស្តាំនៃអេក្រង់របស់អ្នក។

ជំពូកទាំងអស់នៅក្នុងសៀវភៅណែនាំនេះបង្កើតបានជាចំណេះដឹងដែលបានណែនាំនៅក្នុងជំពូកមុន ៗ​ ។ **​អ្នកអាចរៀនចំនុចសំខាន់ៗ​ របស់​ React បាននៅក្នុង​ជំពូក​ គំនិតចម្បង តាមលំដាប់លំដោយដែលមាននៅក្នុងតារាងមាតិកា** ឧទាហរណ៍​ [“ការណែនាំស្តីអំពី JSX”](/docs/introducing-jsx.html) គឺជាមេរៀនបន្ទាប់ពីមេរៀននេះ។

## ការសន្មត់កម្រិតចំណេះដឹង {#knowledge-level-assumptions}

React គឺបណ្ណាល័យរបស់ JavaScript ដូចនេះយើងសន្មត់ថាលោកអ្នកមានមូលដ្ឋានគ្រឺះ JavaScript។ **ប្រសិនបើអ្នកមិនមានទំនុកចិត្តខ្លាំងលើ JavaScript យើងសូមណែនាំអោយ [ទៅមើលមេរៀនរបស់ Javascript សិន](https://developer.mozilla.org/en-US/docs/Web/JavaScript/A_re-introduction_to_JavaScript) ដើម្បីដឹងពីកម្រិតចំណេះដឹងរបស់អ្នក** និងអាចអោយអ្នកយល់ពីការណែនាំនេះជៀសវាងការភ័ន្តច្រលំ។ វាអាចចំណាយពេលត្រឹមតែ ៣០ នាទី ទៅ ១ម៉ោង ប៉ុន្តែវាអាចអោយអ្នកមិនមានអារម្មណ៏ថារៀន React និង​ JavaScript ស្របពេលតែមួយ។

>ចំណាំ
>
>នៅក្នុង​ការ​ណែនាំ​នេះអាចនឹង​មានការ​ប្រើ​ប្រាស់​ Syntax ថ្មីៗ​របស់ JavaScript នៅក្នុងឧទាហរណ៍​មួយចំនួន។ ប្រសិនបើអ្នកមិនបាន​ប្រើប្រាស់ JavaScript​ ក្នុងរយៈពេលប៉ុន្មានឆ្នាំ​ចុងក្រោយ, [ចំណុចទាំងបីនេះ](https://gist.github.com/gaearon/683e676101005de0add59e8bb345340c) អាចជួយអ្នកបានច្រើន។


## តោះចាប់ផ្តើម {#lets-get-started}

សូមបន្តអូសចុះក្រោម អ្នក​នឹង​ឃើញតំណភ្ជាប់ទៅកាន់មេរៀនបន្ទាប់ [មេរៀនបន្ទាប់](/docs/introducing-jsx.html) ស្ថិតនៅខាងស្តាំនៃបាតកថារបស់គេហទំព័រ។


