Gorrila React Hooks Receipts

Gorilla is Korean barbecue tacos truck that makes thousands of hungry customers happy every year.
Their CEO is thinking of updating their short order tracking system using React.
Build a prototype of this short order receipts tracker.

Part 1: Get Started
Spin up a new create-react-app called 'gorrila'.

Part 2: Sample Receipts
You'll be rendering some sample receipts: Hint: You need to create a records component that holds the data below.
const receipt1 =
  {
    person: 'Andre',
    order: {
      main: 'Burrito',
      protein: 'Organic Tofu',
      rice: 'Purple Rice',
      sauce: 'Green Crack',
      toppings: [
        'Baby Bok Choy', 'Cucumber Kimchi'
      ],
      drink: 'Korchata',
      cost: 22
    },
    paid: false
  }
const receipt2 = {
  person: 'Katelyn',
  order: {
    main: 'Rice Bowl',
    protein: 'Ginger Soy Chix',
    rice: 'Sticky Rice',
    sauce: 'Korilla',
    toppings: [
      'Yuzu Pickled Sweet Pepper', 'Kale'
    ],
    drink: 'Korchata',
    cost: 19
  },
  paid: false
}
const receipt3 = {
  person: 'Bruno',
  order: {
    main: 'Salad Bowl',
    protein: 'Organic Tofu',
    rice: 'none',
    sauce: "K'lla",
    toppings: [
      'Blue Potato Salad', 'Pico De Gallo', 'Red Kimchi'
    ],
    drink: 'Sparkling Blood Orange Soda',
    cost: 20
  },
  paid: true
}
Add the receipts to the state of the app:
const [receipts, setReceipts] = useState(receipts)


Make a Receipt component that renders the first receipt's
person
order
main
protein
rice
sauce
drink
cost
Hungry for More: render the toppings
Add the next two receipts to state and make two more Receipt components so that you get a view like this (a little css provided for clarity, but not required)
 

 
Part 3: Refactor for Dynamic Rendering
3 receipts is pretty limiting. Let's put them in an array and then map over them for rendering.
Update your code so it renders the same, but instead of hard coding 3 receipts, it maps over the array.
const receipts = [
  {
    person: 'Steve',
    order: {
      main: 'Burrito',
      protein: 'Organic Tofu',
      rice: 'Purple Rice',
      sauce: 'Green Crack',
      toppings: [
        'Baby Bok Choy', 'Cucumber Kimchi'
      ],
      drink: 'Korchata',
      cost: 22
    },
    paid: false
  },
  {
    person: 'Maddy',
    order: {
      main: 'Rice Bowl',
      protein: 'Ginger Soy Chix',
      rice: 'Sticky Rice',
      sauce: 'Korilla',
      toppings: [
        'Yuzu Pickled Sweet Pepper', 'Kale'
      ],
      drink: 'Korchata',
      cost: 19
    },
    paid: false
  },
  {
    person: 'Derrick',
    order: {
      main: 'Salad Bowl',
      protein: 'Organic Tofu',
      rice: 'none',
      sauce: "K'lla",
      toppings: [
        'Blue Potato Salad', 'Pico De Gallo', 'Red Kimchi'
      ],
      drink: 'Sparkling Blood Orange Soda',
      cost: 20
    },
    paid: true
  }
]
 
Hungry For More
Add a click event on the receipt that changes the value of paid from false to true. Once clicked the receipt should immediately disappear from the browser view
You'll have to research on your own...
How do you style react components within react?
A nice place to start
But also, why would one style components...rather than use a good old css file?

