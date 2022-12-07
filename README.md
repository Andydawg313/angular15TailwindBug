**When using tailwind with angular 15 a bug occurs with an outlined mat-form-field > input where clicking into it will cause a border-right to appear at the end of the floating label**


What the bug looks like

![bug](https://user-images.githubusercontent.com/105505694/206233258-5f0759c7-de3b-47ae-be8d-621d53c1eb04.png)


The border is dependent on the text length of the label

![bug++](https://user-images.githubusercontent.com/105505694/206233935-84d4218a-0d66-4f4a-b3fe-ae847abd777a.png)


Removing the Tailwind base variable fixes the issue `styles.scss` line 5

![css](https://user-images.githubusercontent.com/105505694/206234279-8553154f-e86f-4a52-9c79-ae1601aea0a8.png)


![fixed](https://user-images.githubusercontent.com/105505694/206234634-68b743b6-d1df-4687-9747-9ec96a390fc8.png)
