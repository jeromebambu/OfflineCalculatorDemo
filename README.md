#Bambu Offline Calculator Service #

An example calculator service that will perform offline calculation

### How do I get set up? ###

* Install this sdk in your react or react native project

  ```
  npm install https://github.com/jeromebambu/OfflineCalculatorDemo
  ```

* If using react native, link realm into the project

  ```
  react-native link realm
  ```

* Example Usage

  Import the sdk in your project

  ```
  import KidsEducationCalc from 'kidseducationcalculator'
  ```

  Initialize the sdk inside the constructor

  ```
  export default class App extends Component<Props> {
    constructor() {
      super()
      this.kidsEducation = new KidsEducationCalc();
    }
  ```

  Call Available Methods exposed by the sdk
  * GET university Education Cost
  
    ```
    const data = this.kidsEducation.getUniversityCost();
    console.log(data); // contains an array of object
    ```
  
  * Calculate Kids University Cost
  
    ```
    const payload = {
        age: 18,
        gender: "male",
        universityId: 4,
        medicine: "yes"
      }
      const data = this.kidsEducation.universityCostCalculator(payload);
      console.log(data);
    ```


### Who do I talk to? ###

* Repo owner or admin