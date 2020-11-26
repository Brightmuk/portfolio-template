# Portfolio template ⚡️ [![GitHub](https://img.shields.io/github/license/Brightmuk/portfolio-template?color=blue)](https://github.com/Brightmuk/portfolio-template/blob/master/LICENSE.md) ![GitHub stars](https://img.shields.io/github/stars/Brightmuk/portfolio-template) ![GitHub forks](https://img.shields.io/github/forks/Brightmuk/portfolio-template)

## A portfolio template

<h2 align="center">
  <img src="https://github.com/Brightmuk/portfolio-template/images/screenshots/home-screenshot.png" alt="Simplefolio" width="600px" />
  <br>
</h2>




## Features

⚡️ Modern UI Design 
⚡️ One Page Layout\
⚡️ Styled  Custom CSS\
⚡️ Fully Responsive\
⚡️ Valid HTML5 & CSS3\
⚡️ Well organized documentation

To view a demo example, **[click here](https://brightmuk.github.io/portfolio-template/)**\



## Getting Started 🚀

clone the respository or download the zip file. Launch the index file in your browser and your good to go.




## Template Instructions:

### Step 1 - STRUCTURE


```html
<!-- **** Header section you can customise your own links as per your desire **** -->
    <div class="header">
        <nav class="navbar">
            <div class="max-width">
                <div class="logo"><a href="#">B<span>D</span></a></div>
                <ul class="menu">
                    <li><a href="#home">Home</a></li>
                    <li><a href="#about">About</a></li>
                    <li><a href="#skills">Skills</a></li>
                    <li><a href="#projects">Projects</a></li>
                    <li><a href="#contact">Contact</a></li>
                </ul>
                <div class="menu-btn">
                    <i class="fas fa-bars"></i>
                </div>
            </div>
        </nav>
        <div class="progress-container">
            <div class="progress-bar" id="myBar"></div>
          </div>
    </div>
<!-- /END Header Section -->
```

### Home Section
- On `<img>` tag, fill the `src` property with your profile picture, your picture must be located inside `images/` folder.
- On `<p>` tag with class-name `.home-content.text-2`, include information about you
 - On `.home-social <a >` tags add the link to your social accounts. You can also add a social following that convention. 
```html
    <!-- home section start -->
    <section class="home" id="home" style="background-image: url(images/tree-background.jpg);">
    <div class="max-width">
        <div class="home-content">
            <div class="text-1">Hello, I am </div>
            <div class="text-2">Bright</div>
            <div class="text-3">And I,m a<span> Designer</span><span></span><span></span></div>
            <a href="#contact" class="contact-me">Lets talk</a>
        </div>

    </div>
    <ul class="home-social">
            
        <li>
            <a href=""><i class="fab fa-github" aria-hidden="true"></i><span>Github</span></a>
        </li>
        <li>
            <a href=""><i class="fab fa-instagram" aria-hidden="true"></i><span>Instagram</span></a>
        </li>
        <li>
            <a href="">L<i class="fab fa-linkedin" aria-hidden="true"></i><span>Linkedin</span></a>
        </li>
       
    </ul>
</section>
```

### About Section

- On `.column-right .text` add your personal info
- On `.column-right <a>` add a downloadable link to your cv
```html
    <!-- about section start    -->
    <section class="about" id="about"> 
        <div class="max-width">
            <h2 class="title ">About me</h2>
            <div class="about-content">
                <div class="column left">
                    <img src="images/profile.jpg" alt="">
                    <!-- image credits : Image by <a href="https://pixabay.com/users/stocksnap-894430/?utm_source=link-attribution&amp;utm_medium=referral&amp;utm_campaign=image&amp;utm_content=2584168">StockSnap</a> from <a href="https://pixabay.com/?utm_source=link-attribution&amp;utm_medium=referral&amp;utm_campaign=image&amp;utm_content=2584168">Pixabay</a>-->
                </div>
                <div class="column right">
                    <div class="text">Im Bright a <span>designer</span></div>
                    <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Quibusdam voluptatum inventore hic laborum vel veritatis ratione rem atque necessitatibus, asperiores voluptas minus in. Incidunt consequuntur explicabo amet quaerat architecto! Qui.</p>
                    <a href="">Download cv</a>
                </div>
            </div>
        </div>
    </section>
```
### Skills section

- Each skill set is wrapped by a card. A card has a foreground and a card content that is revealed when mouse hovers on it. 
- On the card foreground is the skill set name : `.foreground .text` e.g Web design.
- In the `card-content` there are percentage charts `single-chart` for a particular skill percentage indication.
- To set your custom percentage on  a skill, change the following:
- 1. `stroke dashray` e.g for 10% set it to `stroke-dasharray="10, 100"`. The first number is the percentage.
- 2. `.percentage` to your desired oercentage.


```html

        <!-- skills section start    -->
        <section class="skills" id="skills"> 
            <div class="max-width">
                <h2 class="title ">My skills</h2>
                <div class="skills-content">
                    <div class="card"> 
                        <div class="foreground">
                            <i class="fas fa-code"></i>
                            <div class="text">Web Design</div>
                        </div>                  
                        <div class="card-content">
                            <div class="label-one"></div> 
                            <div class="label-two"></div> 
                            
                                <span class="tags">Ui/Ux & backend development</span>
                                <div class="flex-wrapper">
                                    <div class="single-chart">
                                      <svg viewbox="0 0 36 36" class="circular-chart orange">
                                        <path class="circle-bg"
                                          d="M18 2.0845
                                            a 15.9155 15.9155 0 0 1 0 31.831
                                            a 15.9155 15.9155 0 0 1 0 -31.831"
                                        />
                                        <path class="circle"
                                          stroke-dasharray="80, 100"
                                          d="M18 2.0845
                                            a 15.9155 15.9155 0 0 1 0 31.831
                                            a 15.9155 15.9155 0 0 1 0 -31.831"
                                        />
                                        <text x="18" y="20.35" class="percentage">80%</text>
                                      </svg>
                                      <div class="technology">HTML/CSS</div>
                                    </div>
                                    
                                    <div class="single-chart">
                                      <svg viewbox="0 0 36 36" class="circular-chart green">
                                        <path class="circle-bg"
                                          d="M18 2.0845
                                            a 15.9155 15.9155 0 0 1 0 31.831
                                            a 15.9155 15.9155 0 0 1 0 -31.831"
                                        />
                                        <path class="circle"
                                          stroke-dasharray="70, 100"
                                          d="M18 2.0845
                                            a 15.9155 15.9155 0 0 1 0 31.831
                                            a 15.9155 15.9155 0 0 1 0 -31.831"
                                        />
                                        <text x="18" y="20.35" class="percentage">70%</text>
                                      </svg>
                                      <div class="technology">JAVASCRIPT</div>
                                    </div>

                            </div>
                            <div class="flex-wrapper">
                                
                                <div class="single-chart">
                                  <svg viewbox="0 0 36 36" class="circular-chart green">
                                    <path class="circle-bg"
                                      d="M18 2.0845
                                        a 15.9155 15.9155 0 0 1 0 31.831
                                        a 15.9155 15.9155 0 0 1 0 -31.831"
                                    />
                                    <path class="circle"
                                      stroke-dasharray="60, 100"
                                      d="M18 2.0845
                                        a 15.9155 15.9155 0 0 1 0 31.831
                                        a 15.9155 15.9155 0 0 1 0 -31.831"
                                    />
                                    <text x="18" y="20.35" class="percentage">60%</text>
                                  </svg>
                                  <div class="technology">NODEJS</div>
                                </div>
                                <div class="single-chart">
                                    <svg viewbox="0 0 36 36" class="circular-chart blue">
                                      <path class="circle-bg"
                                        d="M18 2.0845
                                          a 15.9155 15.9155 0 0 1 0 31.831
                                          a 15.9155 15.9155 0 0 1 0 -31.831"
                                      />
                                      <path class="circle"
                                        stroke-dasharray="60, 100"
                                        d="M18 2.0845
                                          a 15.9155 15.9155 0 0 1 0 31.831
                                          a 15.9155 15.9155 0 0 1 0 -31.831"
                                      />
                                      <text x="18" y="20.35" class="percentage">60%</text>
                                    </svg>
                                    <div class="technology">ANGULAR</div>
                                  </div>
                        </div>
                        <br>
                        <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Consequatur, quam dele </p>
                        </div>
                    </div>
                    <div class="card">  
                        <div class="foreground">
                            <i class="fas fa-mobile"></i>
                            <div class="text">Mobile App Design</div> 
                        </div> 
                        <div class="card-content"> 
                        <div class="label-one"></div> 
                        <div class="label-two"></div>  
                        <span class="tags">Ui/Ux & backend development</span>  
                        <div class="flex-wrapper">
                            <div class="single-chart">
                              <svg viewbox="0 0 36 36" class="circular-chart orange">
                                <path class="circle-bg"
                                  d="M18 2.0845
                                    a 15.9155 15.9155 0 0 1 0 31.831
                                    a 15.9155 15.9155 0 0 1 0 -31.831"
                                />
                                <path class="circle"
                                  stroke-dasharray="60, 100"
                                  d="M18 2.0845
                                    a 15.9155 15.9155 0 0 1 0 31.831
                                    a 15.9155 15.9155 0 0 1 0 -31.831"
                                />
                                <text x="18" y="20.35" class="percentage">60%</text>
                              </svg>
                              <div class="technology">DART</div>
                            </div>
                            
                            <div class="single-chart">
                              <svg viewbox="0 0 36 36" class="circular-chart green">
                                <path class="circle-bg"
                                  d="M18 2.0845
                                    a 15.9155 15.9155 0 0 1 0 31.831
                                    a 15.9155 15.9155 0 0 1 0 -31.831"
                                />
                                <path class="circle"
                                  stroke-dasharray="20, 100"
                                  d="M18 2.0845
                                    a 15.9155 15.9155 0 0 1 0 31.831
                                    a 15.9155 15.9155 0 0 1 0 -31.831"
                                />
                                <text x="18" y="20.35" class="percentage">20%</text>
                              </svg>
                              <div class="technology">JAVA</div>
                            </div>
                            <br>
                    </div>          
                    <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Consequatur, quam dele </p>                        
                        </div>
                    </div>
                    <div class="card">  
                        <div class="foreground">
                            <i class="fas fa-paint-brush"></i>
                            <div class="text">Graphics Design</div>
                        </div>  
                        <div class="card-content">  
                        <div class="label-one"></div> 
                        <div class="label-two"></div> 
                        <span class="tags">Visual art development</span> 
                            <div class="logos-wrapper">
                                <div class="single-logo">
                                    <img class="logos" src="images/adobe-photoshop.jpg">   
                                    <div class="logo-name">Adobe Photoshop</div>
                                </div>
                                <br>
                                <div class="single-logo">
                                    <img class="logos" src="images/adobe-illustrator.png">
                                    <div class="logo-name">Adobe Illustrator</div>
                                </div>
                              <br>

                            </div>                              
                        
                            <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Consequatur, quam dele </p>                        
                    </div>
                </div>               
                </div>
            </div>
        </section>
```


### Projects Section
- Each project is housed by a card named `.card1, .card2 and .card 3`.
- The project image is in the `<img ` referencing images form `images/` folder.
- Add your project link in `<a href=""`

```html
       <!-- projects section starts here -->
        <section class="projects" id="projects">
            <div class="max-width">
                <h2 class="title">My Projects</h2>
                <div class="projects-content">
                       
                  <div class="project-cards">
                    <div class="card card1">
                        <div class="container">
                            <img src="images/blog-ui-desktop.png" alt="las vegas">
                        </div>
                        <div class="details">
                            <h3>Nairobi</h3>
                            <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Praesentium dignissimos, minus aperiam adipisci exercitationem.</p>
                            <a href="" class="project-link">View</a>
                        </div>
                    </div>
                    <div class="card card2">
                        <div class="container">
                            <img src="images/dashboard-ui-desktop.png" alt="New York">
                        </div>
                        <div class="details">
                            <h3>New York</h3>
                            <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Praesentium dignissimos, minus aperiam adipisci exercitationem.</p>
                            <a href="" class="project-link">View</a>
                        </div>
                    </div>
                    <div class="card card3">
                        <div class="container">
                            <img src="images/portfolio-ui-desktop.png" alt="Singapore">
                        </div>
                        <div class="details">
                            <h3>Beijing</h3>
                            <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Praesentium dignissimos, minus aperiam adipisci exercitationem.</p>
                            <a href="" class="project-link">View</a>
                        </div>
                    </div>
                </div>
                </div>

  
            </div>
        </section>

```

### Contact Section

- The contact form send an email to you from the portfolio.
* prerequisites
- Follow the instructions in this link 
 **[click here](https://support.google.com/accounts/answer/185833?hl=en)**
 or watch this video  **[click here](https://youtu.be/i2eXkSKjl0A)**

- You will be able to enable app passwords and a password will be provied for you.

- Once you get an app password open the `js/scripts.js` file
- change the email address and passwords respectively in this function and mails will be sent to you instantly.
```js
//contact form submission
document.querySelector('.contact-form').addEventListener('submit',submitForm);
function submitForm(e){
  e.preventDefault();

  let name = document.querySelector('.name').value;
  let email = document.querySelector('.email').value;
  let message = document.querySelector('.message').value;

  document.querySelector('.contact-form').reset();

  Email.send({
    Host: 'smtp.gmail.com',
    Username: '<your email address>',
    Password: '<your password>',
    To: '<your email address>',
    From: '<your email address>',
    Subject: `${name} has sent you a message from your portfolio`,
    Body: `Name:${name} <br> Email: ${email}<br>  ${message}`,

  }).then((message)=>showAlert())
}
```

```html
    <!-- contact me section -->
        <section class="contact" id="contact">
          <div class="max-width">
            <h2 class="title">Contact me</h2>
            <div class="contact-content">
              <form class="contact-form" method="POST">

                <label for="name">Name</label>
                <input type="text" class="name" name="name" placeholder="Your name.." required>
                <label for="email">Email</label>
                <input type="text" class="email" name="email" placeholder="Your email.." required>

            
                <label for="message">Subject</label>
                <textarea class="message" name="message" placeholder="Write something.." style="height:200px" required></textarea>
            
                <input type="submit" value="Submit">
                <div class="alert mail-not-sent">Your message has been sent !</div>
              </form>
              </div>
              </div>
        </section>

```


## Technologies used 🛠️

- [smtpjs](https://smtpjs.com/v3/smtp.js) - Smtpjs to send mails
- [google fonts](https://fonts.googleapis.com/css2?family=Poppins&display=swap) - You can use your custom font

## Authors

- **Bright Muk** - [https://github.com/Brightmuk](https://github.com/Brightmuk)


## License 📄

This project is licensed under the MIT License - see the [LICENSE.md](LICENSE.md) file for details

