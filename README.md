# TO DEVELOP A PORTFOLIO USING REACT FRAMEWORK
## PROGRAM:
```
DEVELOPED BY: RITHIGA SRI.B
REGISTER NUMBER:212221230083
```
### App.js
```
import React from 'react';
import CV from './CV';


function App() {
  return (
    <div>
      <CV></CV>
    </div>
  );
}

export default App;
```
### CV.js
```
import React,{useRef} from "react";
import './CV.css';
import photo from './photo.jpeg';

const CV=()=>{

    const objRef=useRef(null);
    const scrollToObj=()=>{
        objRef.current.scrollIntoView({ behavior: 'smooth' });
    }
    const aboutRef=useRef(null);
    const scrollToAbout=()=>{
        aboutRef.current.scrollIntoView({behavior:'smooth'});
    }
    const skillRef=useRef(null);
    const scrollToSkill=()=>{
        skillRef.current.scrollIntoView({behavior:'smooth'});
    }
    const expRef=useRef(null);
    const scrollToExp=()=>{
        expRef.current.scrollIntoView({behavior:'smooth'});
    }
    const eduRef=useRef(null);
    const scrollToEdu=()=>{
        eduRef.current.scrollIntoView({behavior:'smooth'});
    }
    const contactRef=useRef(null);
    const scrollToContact=()=>{
        contactRef.current.scrollIntoView({behavior:'smooth'});
    }
    return(
        <body>
            <div className="top">
                <div className="head"><a href="#obj" onClick={scrollToObj}>OBJECTIVE</a></div>
                <div className="head"><a href="#abt" onClick={scrollToAbout}>ABOUT</a></div>
                <div className="head"><a href="#skill" onClick={scrollToSkill}>SKILLS</a></div>
                <div className="head"><a href="#exp" onClick={scrollToExp}>EXPERIENCE</a></div>
                <div className="head"><a href="#edu" onClick={scrollToEdu}>EDUCATION</a></div>
                <div className="head"><a href="#contact" onClick={scrollToContact}>CONNECT ME</a></div>
            </div>
            <center>
                <img src={photo} alt="" className="image"></img>
                <h1 style={{color:"white"}}>RITHIGA SRI.B</h1>
                <h2 style={{color:"white"}}>Data Scientist</h2>
            </center>
            
            <section  ref={objRef} id="obj">
                <div className="heading">
                    OBJECTIVE
                </div>
                <div className="content">
                    <p style={{padding:"15px"}}>To leverage my strong analytical 
                    and technical skills as a data scientist, applying advanced 
                    statistical and machine learning techniques to extract 
                    actionable insights from complex datasets. I aim to contribute 
                    to data-driven decision-making processes and drive meaningful 
                    business outcomes by effectively communicating data-driven 
                    solutions to stakeholders. With a passion for continuous learning 
                    and a curiosity-driven mindset, I strive to stay at the forefront 
                    of data science advancements and make a significant impact in the 
                    field of data-driven innovation.</p>
                </div>
            </section>
            <section ref={aboutRef} id="abt">
                <div className="heading">
                    ABOUT
                </div>
                <div className="elements">
                    <div style={{marginLeft:"240px"}}></div>
                    <div className="b1">Age</div>
                    <div className="b2"><p>20 years</p></div>
                    <div className="b1">Email-Id</div>
                    <div className="b2"><p>rithigasri383@gmail.com</p></div>
                
            </div>
            <div className="elements">
                <div style={{marginLeft:"240px"}}></div>
                <div className="b1">Phone Number</div>
                <div className="b2"><p>7305328312</p></div>
                <div className="b1">Address</div>
                <div className="b2"><p>Enclave Garden,Chennai</p></div>
                
            </div>
            <div class="elements">
                <div style={{marginLeft:"240px"}}></div>
                <div className="b1">Languages</div>
                <div className="b2"><p>Tamil,English</p></div>
                <div className="b1">Date Of Birth</div>
                <div className="b2"><p>03.08.2003</p></div>
                
            </div>
            <div style={{marginBottom:"30px"}}></div>
            </section>
            <section ref={skillRef} id="skill">
                <div className="heading">
                    SKILLS ACQUIRED
                </div>
                <div className="container">
                    <div className="box">
                        <div className="division division1">Technical Skills</div>
                        <div className="division division2">
                            <ul>
                                <li>Programming</li>
                                <li>Statistics and Mathematics</li>
                                <li>Machine Learning</li>
                                <li>Data Manipulation and Analysis</li>
                                <li>Data Visualization</li>
                            </ul>
                        </div>
                    </div>
                    <div className="box">
                        <div className="division division3">Soft Skills</div>
                        <div className="division division4">
                            <ul>
                                <li>Analytical Thinking</li>
                                <li>Communication Skills</li>
                                <li>Curiosity and Learning Mindse</li>
                                <li>Collaboration and Teamwork</li>
                                <li>Business Acumen</li>
                            </ul>
                        </div>
                    </div>
                </div>
            </section>
            <section ref={expRef} id="exp">
                <div className="heading">
                    EXPERIENCE
                </div>
                <div className="content" style={{padding:"5px"}}>
                    <ul>
                        <li>Monolith Research and Development Center<i>(Jan-Feb 2023)</i></li>
                        <li>Teachnook <i>(Feb-Mar 2023)</i></li>
                    </ul>
                </div>
            </section>
            <section ref={eduRef} id="edu">
                <div className="heading">
                    EDUCATION
                </div>
                <div className="content" style={{padding:"5px"}}>
                    <ul>
                        <li>SSLC - 96.4% Velammal Vidhyshram<i>(2018-2019)</i></li>
                        <li>SSLC - 90.0% Velammal Vidhyshram <i>(2020-2021)</i></li>
                        <li>B.Tech Artificial Intelligence and Data Science <i>(2021-2025)</i></li>
                    </ul>
                </div>
            </section>
            <section ref={contactRef} id="contact">
                <div className="heading">
                    CONNECT ME
                </div>
                <div style={{display:"flex",justifyContent:"space-evenly",margin:"30px"}}>
                    <div class="button"><a href="#git">Github</a></div>
                    <div class="button"><a href="#link">LinkedIn</a></div>
                    <div class="button"><a href="#mail">Gmail</a></div>
                </div>
            
            </section>
        </body>
    )
}

export default CV;
```
### CV.css
```
body {
    background-image: url('https://i.pinimg.com/236x/ac/dc/1b/acdc1b5563a3d1e172eb7d8b6e90bd58.jpg');
    background-size: cover; 
    margin:10px;
    
    
}
section{
    margin-top: 50px;
}
a {
    text-decoration: none; 
    font-size: 18px;
    color:black;
    
}
.button a{
    color:white;
}
.top
{
    display: flex;
    color: white;
    font-family: monospace;
    justify-content: space-between;
    margin-bottom: 15px;
    background-color: lightgreen;
    padding:15px;
}
.head{
    background-color:black;
    width:100px;
    margin:3px;
    padding:5px;
    border-radius:10px;
    text-align:center;
}
.head a
{
    color:white;
}
.head:hover{
    background-color:#483d8b; 
}

.image
{
    border-radius: 10px;
    width:200px;
    height:250px;
    margin-bottom: 30px;
}
.heading
{
    height:40px;
    width:70%;
    margin:auto;
    background-color:lightgreen;
    color:black;
    border-radius:10px;
    box-shadow: 0 0 3px white;
    border:2px solid black;
    font-family: monospace;
    font-size: 30px;
    display: flex;
    align-items: center;
    justify-content: center;

}

.content
{
    width:70%;
    margin:auto;
    background-color:whitesmoke;
    margin-top:15px;
    border-radius:10px;
    font-family:'Gill Sans', 'Gill Sans MT', Calibri, 'Trebuchet MS', sans-serif;
    text-align: justify;
    font-size: 20px;
    margin-bottom: 30px;
}
.container {
    display: flex;
    margin-left:200px;
    margin-right:200px;
  }
  
  .box {
    flex: 1;
    display: flex;
    flex-direction: column;
    padding: 20px;
  }
  
  .division {
    flex: 1;
    display: flex;
    align-items: center;
    justify-content: center;
    color:black;
    
  }
  
  .division1 {
    background-color:darkslateblue;
    font-size:30px;
    font-family:monospace;
    border-radius:10px 10px 0 0;
    padding: 3px;
    font-weight: bold;
    color:white;
    
  }
  
  .division2 {
    background-color: #ffffff;
    font-size:20px;
    font-family:Cambria, Cochin, Georgia, Times, 'Times New Roman', serif;
    border-radius: 0 0 10px 10px;
    padding:3px;
    line-height: 30px;
    
  }
  
  .division3 {
    background-color:darkslateblue;
    font-size:30px;
    font-family:monospace;
    border-radius:10px 10px 0 0;
    padding: 3px;
    font-weight: bold;
    color:white;
  }
  
  .division4 {
    background-color: #ffffff;
    font-size:20px;
    font-family:Cambria, Cochin, Georgia, Times, 'Times New Roman', serif;
    border-radius: 0 0 10px 10px;
    padding:3px;
    line-height: 30px;
  }

  .b1
{
    margin-top:50px;
    width:150px;
    height:50px;
    background-color: darkslateblue;
    overflow: hidden;
    color:white;
    font-family: monospace;
    font-size: 20px;
    display: flex;
    align-items: center;
    justify-content: center;
    border-radius: 10px 0 0 10px;
}
.elements
{
    display: flex; 
     
}
.b2
{
    height:50px;
    width:250px;
    background-color: white;
    margin-top:50px;
    margin-right: 150px;
    color:Black;
    font-family:'Trebuchet MS', 'Lucida Sans Unicode', 'Lucida Grande', 'Lucida Sans', Arial, sans-serif;
    font-size: 20px;
    padding-left: 10px;
    padding-right: 10px;
    display: flex;
    align-items: center;
    text-align: justify;
    border-radius: 0 10px 10px 0;
}

.button
{
    background-color:darkslateblue;
    color:white;
    font-family: monospace;
    padding: 15px;
    border-radius: 20px;
    width:70px;
    text-align: center;
}
```

### OUTPUT:
![image](https://github.com/Rithigasri/Portfolio-React/assets/93427256/218df701-874d-40ee-a1f3-4435aba8d607)  
![image](https://github.com/Rithigasri/Portfolio-React/assets/93427256/a570d13e-a355-47e9-8a69-48ce3b90f5c2)  
![image](https://github.com/Rithigasri/Portfolio-React/assets/93427256/ad6c49c8-400b-47e3-b466-65f26e767b7c)
## RESULT:
Thus, a portfolio is created using react framework.

