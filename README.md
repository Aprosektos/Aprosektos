`class münür {
  constructor(...options) {
    this.height = "1.85"
    this.weight = "63"
    this.type = "human"
    this.job = "coder"
    this.sex = "male"
  }
}

class CreateMan extends münür {
  constructor(...options) {
    super(options);
  }
  
  private _eating() {
    void "eating 🍔 🍟 🍗 🥤"
  }
  
  private _coding() {
    void "coding... ❤️"
  }
  
  private _sleep(ms) { return new Promise(resolve => setTimeout(resolve, ms)) }
  
  async createDay() {
    this._eating()
    this._coding()
    await this._sleep(18000000)
    
    this.createDay()
  }
  
}

let münür = new CreateMan()
münür.createDay();
`
