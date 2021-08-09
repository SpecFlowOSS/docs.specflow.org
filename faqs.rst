Frequently Asked Questions
==========================

.. raw:: html

   <embed>
      <style>
         #faq-container #search-bar input,
         #faq-container #search-bar select
         {
            border-radius: 50px;
            padding: 6px 12px;
            border-color: #2472a4;
            height: 1.8rem;
         }

         #faq-container #search-bar {
            margin-bottom: 0.5rem;
         }

         #faq-container #search-bar label {
            display: inline-block;
         }

         #faq-container h3 { 
            color: #8588b6;
            margin-bottom: 0.5rem;
            cursor: pointer;
         }

         #faq-container .question {
            margin-bottom: 0.7rem;
            max-width:800px;
         }

         #faq-container .question strong {
            cursor: pointer;
            display: block;
            text-indent: -14px;
            margin-left: 14px;
            margin-bottom: 5px;
            margin-top: 15px;
         }

         #faq-container .question strong::before {
            content: "+";
            color: #8588b6;
            font-weight: bold;
            font-size: 1.2rem;
            font-family: monospace;
            margin-right: 0.2rem;
         }
         #faq-container .question.open strong::before {
            content: "-";
         }

         #faq-container section h3::before {
            content: "+";
            color: #808080;
            font-weight: bold;
            font-size: 1.2rem;
            font-family: monospace;
            margin-right: 0.2rem;
         }
         #faq-container section.open h3::before {
            content: "-";
         }

         #faq-container section .questions {
            max-height: 0;
            transition: max-height 300ms cubic-bezier(0, 1, 0, 1);
            overflow: hidden;
         }
         #faq-container section.open .questions {
            max-height: 20000px;
            transition: max-height 300ms ease-in;
         }


         #faq-container .question .answer {
            box-sizing: border-box;
            padding-top: 0.2rem;
            padding-left: 1rem;
            max-height: 0;
            transition: max-height 300ms cubic-bezier(0, 1, 0, 1);
            overflow: hidden;
         }
         #faq-container .question.open .answer {
            max-height: 1000px;
            transition: max-height 300ms ease-in;
         }

         #faq-container .question .answer pre {
            overflow: auto;
            border: 1px solid #8588b6;
            border-radius: 5px;
            padding: 0.5rem;
            background: white;
         }
      </style>
      <div id="faq-container">
         <div id="search-bar">
            <input type="text" id="filter" placeholder="Search the FAQs">
            <Label>
               &nbsp; and/or filter by category
               <select id="group-select">
               
               </select>
            </label>
         </div>
         <div id="faq-sections">
            <section >
               <h3>General</h3>
               <div class="questions">
                  <div class="question">
                     <strong>Is SpecFlow an implementation of Cucumber?</strong>
                     <div class="answer">
                        SpecFlow is using the same Gherkin language to define your Scenarios as Cucumber. It has the same and sometimes more features than Cucumber but is limited to the .NET ecosystem.
                     </div>
                  </div>
                <div class="question">
                     <strong>Can SpecFlow replace unit tests?</strong>
                     <div class="answer">
                        Unit tests are a testing technique, so if you ask if you can replace unit tests that ensure technical excellence with SpecFlow, the answer is no. However, If you are thinking about the unit tests that check for functionality, you can probably use SpecFlow for them. 
                        But since unit tests are usually used for technical excellence, the easy answer is no. 

                     </div>
                  </div>
                <div class="question">
                     <strong>Is it possible to introduce BDD during a project?</strong>
                     <div class="answer">
                     Yes, it is. People understand the purpose and benefits of BDD most of the time rather quickly. 
                     You need to consider that for BDD, typically, the automation part is a bit more complex because we are usually automating the application via an external interface.          
                                            
                     </div>
                  </div>

                <div class="question">
                     <strong>Are there any tools/services recommended for the Discovery and Formulation phase?</strong>
                     <div class="answer">

                     For Discovery:
                     Any tool/service that lets you collaborate in real-time. Examples would be:
                     <br></br>
                    <ul>
                        <li> <a href="https://www.mural.com/" target="_blank" rel="noopener noreferrer">Mural</a></li>
                        <li> <a href="https://miro.com/" target="_blank" rel="noopener noreferrer">Miro</a></li>
                        <li> Google Docs </li>
                        <li> Office 365 </li>
                    </ul>

                     For Formulation:
                     We recommend our own SpecFlow Gherkin Editor. Details can be found <a href="https://specflow.org/tools/online-gherkin-editor/" target="_blank" rel="noopener noreferrer">here</a>                                      
                           
                  </div>
                  </div>                 
                <div class="question">
                     <strong>Should developers use Scenarios as their source of the requirements?</strong>
                     <div class="answer">
                     No. From our experience, when you have only concrete examples for implementing, a developer needs to abstract how the feature works again. Developers need the conceptual definition of the requirement to implement it and use the examples to see if the implementation is doing the correct behavior.            
                                            
                     </div>
                </div>

                <div class="question">
                    <strong>In a typical Scrum iteration, when would the Requirement workshop and Example mapping usually take place? </strong>
                    <div class="answer">
                    As these meetings are about defining your user stories/product backlog entries, they need to happen before planning for a sprint/iteration. One possibility is to hold the Discovery and Example mapping sessions in your refinement meetings.            
                                       
                    </div>

                </div>

                <div class="question">
                    <strong>How would you approach getting everyone involved with tests earlier when this is a big shift from current workflow? </strong>
                    <div class="answer">
                    Don't talk about tests; start talking about concrete examples of how the application should behave. From our experience, there will always be questions for exceptional cases, and they need to be addressed. Convince them that it is better to answer these as early as possible and not when half of the features are already implemented. Depending on the answer, a more extensive rewrite might be needed.            
                                       
                    </div>

                </div>

                <div class="question">
                    <strong>Should the BDD approach only be used for a new project?</strong>
                    <div class="answer">
                    No. You can start with BDD at any time. You can start small by just thinking and writing down the behavior of the application with concrete examples. After that, you can go further with formulating them in Gherkin and somewhen automate them.            
                                       
                    </div>

                </div>

                <div class="question">
                    <strong>What is the difference between Cucumber and Gherkin?</strong>
                    <div class="answer">
                    Gherkin is the language you are using to write and formulate your scenarios.
                    Cucumber is a tool to automate these scenarios on programming languages like Java, JavaScript, Ruby, and a lot more                               
                                   
                   </div>

                </div>

               <div class="question">
                    <strong>Can you give recommendations to approach a Shift Left Testing approach with SpecFlow?</strong>
                    <div class="answer">
                    Check out this <a href="https://support.specflow.org/hc/en-us/community/posts/360015333737-Need-recommendations-for-Shift-Left-Testing-in-Agile" target="_blank" rel="noopener noreferrer">article.</a>                            
                                   
                   </div>

               </div>
                
               <div class="question">
                    <strong>Is it possible to mix SpecFlow tests and standard unit tests in the same VS project?</strong>
                    <div class="answer">
                    Our recommendation is to have two separate projects—one for unit tests and one for SpecFlow scenarios.
                    SpecFlow integrates into the various test runners to be able to enable all its features. Combining SpecFlow tests and standard unit tests may cause some of these features not to function as expected. Before and After TestRun hooks are an example of this.
                                                   
                              
                    </div>

              </div>

              <div class="question">
                    <strong>Is it possible to use SpecFlow+ LivingDoc for .NET Framework projects?</strong>
                    <div class="answer">
                    Yes, it can be used for .NET Framework projects and.NET Core or .NET projects. You only need a .NET Core runtime available to run SpecFlow+ LivingDoc.
                              
                    </div>

              </div>

              <div class="question">
                    <strong>What is the Price/Cost of SpecFlow?</strong>
                    <div class="answer">
                    SpecFlow is free and largely open source! Thanks to the backing of Tricentis. Just give it a go and enjoy our tools.
                    </div>

              </div>

              <div class="question">
                    <strong>Who are the people behind SpecFlow?</strong>
                    <div class="answer">
                    Meet us on any of our webinars or social media. You can read more about us <a href="https://specflow.org/about/" target="_blank" rel="noopener noreferrer">here.</a>
                    </div>

              </div>
              
              <div class="question">
                    <strong>Is SpecFlow actively maintained and supported?</strong>
                    <div class="answer">
                    SpecFlow and the rest of our tools are constantly under development. You can check out our GitHub project, our public roadmap, feature requests, and our webinars to learn about what we are currently working on.
                    </div>

              </div>

            <div class="question">
              <strong>Is SpecFlow suitable for DevOps testing?</strong>
              <div class="answer">
              SpecFlow supports a development technique (BDD) with a heavy focus on testing. The SpecFlow framework uses common unit test runners (nUnit, xUnit, and MSTest) for test execution of its .dlls. It can therefore be very nicely integrated into any build server or automated CI/CD pipeline.
              </div>

            </div>

            <div class="question">
              <strong>What is SpecFlow?</strong>
              <div class="answer">
              SpecFlow allows .NET development teams to define, manage and execute automated acceptance tests as business readable specifications.
              SpecFlow is based on Gherkin language and aims to bridge the communication gap between domain experts and developers. Acceptance tests in SpecFlow follow the BDD paradigm of defining specifications with examples, so that they are also easily understood by non-technical users. Acceptance tests can then be tested automatically as needed, while their specification serves as a living documentation of the system.
              SpecFlow integrates with Visual Studio, but can be also used from the command line (e.g. on a build server).
              SpecFlow has a range of other products under the SpecFlow+  product range. These products add additional functionalities to SpecFlow, such as a Gherkin editor , advanced reporting (LivingDoc) and much more.

              </div>

            </div>
            
            <div class="question">
              <strong>How do I install SpecFlow?</strong>
              <div class="answer">
              To install SpecFlow and SpecFlow+, you first need to <a href="https://docs.specflow.org/projects/getting-started/en/latest/GettingStarted/Step1.html" target="_blank" rel="noopener noreferrer">install the SpecFlow Visual Studio extension.</a>. Once you have done this, you can then add SpecFlow to each of your projects. For more details, see the <a href="https://docs.specflow.org/projects/getting-started/en/latest/index.html" target="_blank" rel="noopener noreferrer">Getting Started article</a>, where you learn how to install and use SpecFlow and also see how sample project works with SpecFlow.
              </div>

            </div>
            
            <div class="question">
              <strong>What is the difference between SpecFlow and SpecFlow+?</strong>
              <div class="answer">
              SpecFlow is open source and covers all your basic needs for managing, automating and testing specifications by example.
              SpecFlow+ is a series of extensions that introduce additional features, such as the <a href="https://specflow.org/tools/online-gherkin-editor/" target="_blank" rel="noopener noreferrer">Gherkin editor</a> for Gherkin specifications, and <a href="https://specflow.org/tools/living-doc/" target="_blank" rel="noopener noreferrer">living documentation</a>. SpecFlow and SpecFlow+ products are free to use. We only ask your to register for a free account using a free Microsoft account.
            
            </div>
            </div>
            <div class="question">
              <strong>Do you have a public product roadmap?</strong>
              <div class="answer">
              Please check our <a href="https://docs.specflow.org/en/latest/roadmap.html" target="_blank" rel="noopener noreferrer">roadmap page</a> for an updated overview of what is coming up and what the team is working on right now.
            
              </div>
            </div>
            <div class="question">
              <strong>How can I contribute to SpecFlow's development?</strong>
              <div class="answer">
              Details on how you can contribute to SpecFlow's development can be found <a href="https://github.com/SpecFlowOSS/SpecFlow/blob/master/CONTRIBUTING.md" target="_blank" rel="noopener noreferrer">here</a>. There are a number of ways you can contribute to SpecFlow such as working on bug fixes, feature requests, and writing documentation.
            
              </div>
            </div>
            <div class="question">
              <strong>I have a feature request, will you implement it?</strong>
              <div class="answer">
              We appreciate any feedback on how you are using SpecFlow and how your experience could be improved. You can submit feedback on our <a href="https://support.specflow.org/hc/en-us/community/topics/360000519178-Feature-Requests" target="_blank" rel="noopener noreferrer">feature request list.</a> We will evaluate all suggestions we receive, and factor this feedback into future development cycles.
              </div>
            </div>
            <div class="question">
            <strong>Who are the developers behind SpecFlow?</strong>
            <div class="answer">
            SpecFlow was originally created by a team at TechTalk, lead by Christian Hassa and Gaspar Nagy, but recently SpecFlow and its add on components, SpecFlow+, are owned and sponsored by <a href="https://www.tricentis.com" target="_blank" rel="noopener noreferrer">Tricentis</a>.
            Since open-source developers from around the world have contributed to the project; an overview can be found here. Please visit our about us page to get to know the team behind SpecFlow.
            
            </div>
          </div>

          <div class="question">
          <strong>Can I use the SpecFlow name for my own projects?</strong>
          <div class="answer">
          We are always happy to see projects that extend SpecFlow’s feature set, and SpecFlow is open source to specifically encourage such contributions from the community. We have however reserved the rights to the name “SpecFlow” as well as the official SpecFlow logo. We need to retain control over this aspect of the project, as we share responsibility for supporting and maintaining SpecFlow, along with all other contributors in the community.
          When naming your project, one of our primary concerns is therefore that the name of your project avoids any confusion concerning project ownership and avoids creating the impression that your project is officially supported by us. 

          
          </div>
        </div>

        <div class="question">
        <strong>How do I enable tracing in SpecFlow?</strong>
        <div class="answer">
        You can enable traces for SpecFlow. Once tracing is enabled, a new SpecFlow pane is added to the output window showing diagnostic messages.
        To enable tracing, select Tools | Options | SpecFlow from the menu in Visual Studio and set Enable Tracing to 'True'.       
        
        </div>
      </div>

      <div class="question">
        <strong>Upgrade error : "Trace listener failed. -> The ScenarioContext...."</strong>
        <div class="answer">
        To resolve this error, make sure you have regenerated the .feature.cs files after upgrading. If you do not do this, you will receive this exception when accessing ScenarioContext.Current.
        <br></br>
        To regenerate these files:<br></br>
        
           1. Open a feature file in your solution. If you see a popup informing you that the feature files were generated with an earlier version of SpecFlow, click on Yes to regenerate these files. Depending on the size of your project, this may take a while.<br></br>
           2. If you are using an earlier version of Visual Studio, you need to force the feature files to be regenerated. Right-click on your project, and select Regenerate Feature Files from the menu.<br></br>       
        
        </div>
      </div>

      <div class="question">
        <strong>Visual Studio error: "Missing [assembly:GeneratorPlugin] attribute"</strong>
        <div class="answer">
        If you are receiving this error, try setting the Generation Mode in SpecFlow to "OutOfProcess". To do so:<br></br>
        
            1.	Select Tools | Options from the menu in Visual Studio.<br></br>
            2.	Select SpecFlow from the list on the left.<br></br>
            3.	Locate the Generation Mode setting and set it to "OutOfProcess".<br></br>
        
        
        </div>
      </div>
        
        <div class="question">
        <strong>Steps are not recognized even though there are matching step definitions</strong>
        <div class="answer">
        The SpecFlow Visual Studio integration caches the binding status of step definitions. If the cache is corrupted, steps may be unrecognised and the highlighting of your steps may be wrong (e.g. bound steps showing as being unbound). To delete the cache: <br></br>    

            1. Close all Visual Studio instances. <br></br>
            2. Navigate to your <i>%TEMP%</i> folder and delete any files that are prefixed with <i>specflow-stepmap-</i>, e.g. <i>specflow-stepmap-SpecFlowProject-607539109-73a67da9-ef3b-45fd-9a24-6ee0135b5f5c.cache.</i><br></br>
            3. Reopen your solution.
        </div>
        </div>

        <div class="question">
        <strong>Visual Studio error: Cannot find custom tool `SpecFlowSingleFileGenerator`</strong>
        <div class="answer">
        If Visual Studio displays the error message <i> Cannot find custom tool 'SpecFlowSingleFileGenerator' on this system</i>, when right-clicking on a feature file and selecting <i>Run Custom Tool</i>, make sure the SpecFlow extension is installed and enabled.
        To enable the extension in Visual Studio, select Tools | Extensions and Updates..., select the "SpecFlow for Visual Studio" extension, then select Enable.
        
        </div>
        </div>
        <div class="question">
        <strong>Unable to find plugin in the plugin search path when saving / generating feature files</strong>
        <div class="answer">
        SpecFlow searches for plugins in the NuGet packages folder. This is detected relative to the reference to TechTalk.SpecFlow.dll. If this DLL is not loaded from the NuGet folder, the plugins will not be found.
            A common problem is that the NuGet folder is not yet ready (e.g. not restored) when opening the solution, but <i>TechTalk.SpecFlow.dll</i> in located in the <i>bin\Debug</i> folder of the project. In this case, Visual Studio may load the assembly from the <i>bin\Debug</i> folder instead of waiting for the NuGet folder to be properly restored. Once this has happened, Visual Studio remembers that it loaded the assembly from <i>bin\Debug</i>, so reopening the solution may not solve this issue. The best way to fix this issue is as follows:<br></br>
            1.	Make sure the NuGet folders are properly restored.<br></br>
            2.	Close Visual Studio.<br></br>
            3.	Delete the bin\Debug folder from your project(s).<br></br>
            4.	Reopen your solution in Visual Studio.<br></br>        
        </div>
        </div>

        <div class="question">
        <strong>How can I contact support?</strong>
        <div class="answer">
        If you have a general issue, suggestion or question concerning SpecFlow products, please visit our <a href="https://support.specflow.org/hc/en-us" target="_blank" rel="noopener noreferrer">support page</a>.       
        </div>
        </div>

        <div class="question">
        <strong>I have a feature request; where can I submit it?</strong>
        <div class="answer">
        Please direct all your feature requests <a href="https://support.specflow.org/hc/en-us/community/topics/360000519178-Feature-Requests" target="_blank" rel="noopener noreferrer">here</a>, where the SpecFlow community gets to add and votes on existing feature requests.
        
        </div>
        </div>

        
    </div>
        </section>

            <section>
               <h3>BDD</h3>
               <div class="questions">
               
            
            <div class="question">
            <strong>How would you best describe the tester role in BDD – would they concentrate on not-automated tests?</strong>
            <div class="answer">
            Yes, using BDD would enable them to have time for more manual testing like exploratory testing or release testing. They need less time to spend on regression testing because the scenarios are automated and can be executed whenever needed.
            But they will also get involved more earlier in the discussions of how a feature should work. With their unique views on requirements and thoughts about concrete examples, testers help identify missing information in the requirements. These examples can then be used for your scenarios.
       
            </div>
            </div>

            <div class="question">
            <strong>Why do most of the people from the IT industry think BDD is a testing tool?</strong>
            <div class="answer">
            We think this happened because the automation part of BDD is the most accessible part of the three phases (Discovery, Formulation, Automation), and you get something concrete out of it. Discovery and Formulation are the complex parts that need adjustments on how you and your team are working.
       
            </div>
            </div>
         </div>   
         </section>


            <section>
               <h3>Writing Scenarios</h3>
               <div class="questions">
               
            <div class="question">
            <strong>Is there an OR keyword?</strong>
            <div class="answer">
            No, there is not. The reason is that the intention of Gherkin is to make it possible for everyone to write understandable scenarios. If there were an Or, there would be branches on how you read a Scenario and add unnecessary complexity. 
       
            </div>
            </div>

            <div class="question">
            <strong>Do Scenarios and Features need to be completely independent?</strong>
            <div class="answer">
            Yes, they need to be independent. Every test runner is running scenarios in a different order. 
       
            </div>
            </div>

            <div class="question">
            <strong>Which is good practice when writing Scenarios? "When I perform an action," or "When a user performs an action."</strong>
            <div class="answer">
            The recommendation is to use the third person form like "When a user performs an action." The reason is that this makes it clear which person/role is the current user. When you write it in the first person, it is not clear which role you are in at the moment. 
       
            </div>
            </div>

            <div class="question">
            <strong>How do you do data-driven testing with an external source like CSV, Excel in Scenarios?</strong>
            <div class="answer">
            You can use SpecFlow.External Data for this. More information <a href="https://docs.specflow.org/projects/specflow/en/latest/Guides/externaldata.html" target="_blank" rel="noopener noreferrer">here</a>.  
       
            </div>
            </div>

            <div class="question">
            <strong>Does Given in the Background replace the Given that would be in the Scenario?</strong>
            <div class="answer">
            No, Background steps are not replacing the Given steps in a scenario. First, the steps in the Background are executed, and then the steps in the Scenario.
       
            </div>
            </div>

            <div class="question">
            <strong>If there are no Given steps, does that affect SpecFlow?</strong>
            <div class="answer">
            No. It is possible to have no Given steps in a scenario.
       
            </div>
            </div>

            <div class="question">
            <strong>How many steps/lines should an ideal Scenario have?</strong>
            <div class="answer">
            It always depends on your application, but if you need to scroll to read a single scenario, you should try to make it shorter.
       
            </div>
            </div>


            <div class="question">
            <strong>Is it acceptable to write a "Given When Then When Then" scenario?</strong>
            <div class="answer">
            No, this is a bad practice. Having multiple "When Then" blocks is a sign that you are testing various behaviors at once. You can probably put every "When Then" block into a different scenario. This makes it also easier to find out what part is broken if the Scenarios start failing.
       
            </div>
            </div>


            <div class="question">
            <strong>What is the difference between a table and a Scenario Outline?</strong>
            <div class="answer">
            <a href="https://docs.specflow.org/projects/specflow/en/latest/Gherkin/Gherkin-Reference.html#scenario-outline" target="_blank" rel="noopener noreferrer">Scenario Outlines</a> and Tables, also called <a href="https://docs.specflow.org/projects/specflow/en/latest/Gherkin/Gherkin-Reference.html#data-tables" target="_blank" rel="noopener noreferrer">Data Tables</a> are two completely different things.
            Scenario Outlines give you the possibility to parameterize your Scenarios so that you don't have to duplicate a Scenario multiple times to showcase minor changes.
            Tables are a parameter for your step definitions. They give you the possibility to pass more parameters to a step definition in a more structured way.
            You can access the Table in a non-typesafe way. To get a more typesafe API, you can use the extension methods in SpecFlow.Assist namespace. You can read more about it <a href="https://docs.specflow.org/projects/specflow/en/latest/Bindings/SpecFlow-Assist-Helpers.html" target="_blank" rel="noopener noreferrer">here</a>.
          
     
            </div>
            </div>

            <div class="question">
            <strong>Is there a way to parameterize a feature the same way as a scenario outline?</strong>
            <div class="answer">
            No, there is not. 
            What is possible is to parameterize all features/scenarios with the <a href="https://docs.specflow.org/projects/specflow-runner/en/latest/Profile/Targets.html" target="_blank" rel="noopener noreferrer">Target- Feature</a> of the SpecFlow+ Runner.

            </div>
            </div>

            <div class="question">
            <strong>Is it possible to use two tables in StepDefinition?</strong>
            <div class="answer">
            No, it is not possible. The main idea is that one step should represent one action. If a step's text indicates more actions than that, it is a sign that the step should be split up.
       
            </div>
            </div>


               </div>
            </section>
            <section>
               <h3>Automation</h3>
               <div class="questions">
                  <div class="question">
                     <strong>How can you have optional parameters in step definitions?</strong>
                     <div class="answer">
                        SpecFlow doesn't support optional parameters in the step definition methods. You have to write two methods, but you can simply call one from the other. 
                        <pre>
      [Given(@"Add two numbers (.*) (.*) (.*)")] 
      public void Testtheconditionwith(string a, string b, string c)
      { 

      } 

      [Given(@"Add two numbers (.*) (.*)")]  
      public void Testtheconditionwith(string a, string b) 
      { 
         Testtheconditionwith(a,b,null) 
      }</pre>
                           </div>
                        </div>

            
               <div class="question">
               <strong>What is the Scenario Context, and in what ways can it be used?</strong>
               <div class="answer">
               It's the best way to share information across a scenario. E.g., you need to save a login name at the beginning of a Scenario and validate it at the end. You would use ScenarioContext to access that info throughout the Scenario.
               </div>
               </div>

               <div class="question">
               <strong>How do you refactor a project that has step definitions that call on other step definitions? </strong>
               <div class="answer">
               The suggestions is to just call the method name itself. E.g: QuestionAskingStepDefinition.ThenTheSuggestionListShouldBeFound()
               </div>
               </div>

               <div class="question">
               <strong>How and when is the ScenarioContext instantiated?</strong>
               <div class="answer">
               It is done automatically by the SpecFlow runtime. You only have to request it via constructor injection to get the correct instance.
               </div>
               </div>

               <div class="question">
               <strong>How many Step definitions can there be for one PageObject class?</strong>
               <div class="answer">
               There is no limit on how many step definitions you can have.
               </div>
               </div>

               <div class="question">
               <strong>How do you group your step definitions in classes?</strong>
               <div class="answer">
               We recommend grouping them by feature/area they are automating.
               </div>
               </div>

               <div class="question">
               <strong>If an 'AND' is used at a step, the Visual Studio plugin creates another 'Given' attribute. </strong>
               <div class="answer">
               There are only Given/When/Then steps. An And step is always of the type in which block they appear. So, if you have And Steps after a Given steps, they are Given steps.
               </div>
               </div>

               <div class="question">
               <strong>How can you execute Features and Scenarios in order?</strong>
               <div class="answer">
               SpecFlow does not influence the execution order of your scenarios. Your test runner handles this. Please check the documentation of your test runner to see if it is possible to run tests in a particular order.
               </div>
               </div>

               <div class="question">
               <strong>Is it possible to create dependencies between tests? </strong>
               <div class="answer">
               No, this is not possible. Execution order is in the hands of the test runner (NUnit, xUnit, MSTest, SpecFlow+ Runner), and SpecFlow can't manipulate this. Currently, no runner supports this use case.
               </div>
               </div>

               <div class="question">
               <strong>Can we pair a particular feature file with only one step definition class?</strong>
               <div class="answer">
               Technically yes, but it is not recommended at all. When you rename the feature title or move a scenario into another file, everything will break.
               </div>
               </div>

               <div class="question">
               <strong>Why should we not use Thread. Sleep?</strong>
               <div class="answer">
               Because the duration of the action you are waiting can differ over time. Somewhen your scenarios will break because the time you wait isn't enough.
               </div>
               </div>

               <div class="question">
               <strong>Should the application code and test code be in different solutions?</strong>
               <div class="answer">
               If possible, it is highly recommended that test code and application code are in the same solution. 
               </div>
               </div>

               <div class="question">
               <strong>Is it a good practice to have a separate Step Definition file for each Feature file?</strong>
               <div class="answer">
               No, and it is not necessary. Step definitions are global. This means you define it per project and not only for a single feature file.
               </div>
               </div>

               <div class="question">
               <strong>What is the difference between the Driver pattern and the PageObject pattern?</strong>
               <div class="answer">
               These two patterns are solving different requirements.
               The Page Object Model is a pattern that is often used to abstract your Web UI with Selenium to automate it easier. More information here <a href="https://docs.specflow.org/projects/specflow/en/latest/Guides/PageObjectModel.html" target="_blank" rel="noopener noreferrer">here</a>.
               The Driver Pattern is an additional layer between your step definitions and your automation code. With it, you can easily reuse your automation logic. More information <a href="https://docs.specflow.org/projects/specflow/en/latest/Guides/DriverPattern.html" target="_blank" rel="noopener noreferrer">here</a>.

               </div>
               </div>

               <div class="question">
               <strong>Are there any hooks for Rules?</strong>
               <div class="answer">
               No, there aren't hooks for Rules.
               </div>
               </div>

               <div class="question">
               <strong>What is the lifetime of fields/members of a step definition class?</strong>
               <div class="answer">
               Every Scenario that gets executed has its own instances of step definition classes.
               A step definition class and all its fields and members are alive and in memory as long as the Scenario in which they were used is executed. After a scenario ended, they are released and not used anymore.

               </div>
               </div>

               <div class="question">
               <strong>Are there any drawbacks or advantages for specific test runners?</strong>
               <div class="answer">
               Every test runner has some unique features. Depending on your needs, choose the appropriate one. You can get an overview at <a href="https://specflow.org/tools/runner/" target="_blank" rel="noopener noreferrer">here</a>
               </div>
               </div>

               <div class="question">
               <strong>Do we need to check in the feature.cs file?</strong>
               <div class="answer">
               No, you do not need to. The `feature.cs` files are generated when the project is built so that they would be generated in a CI/CD pipeline.
               </div>
               </div>

               <div class="question">
               <strong>How do you regenerate the feature code-behind files when you are changing test runner?</strong>
               <div class="answer">
               Rebuild your project that contains SpecFlow and change the test runner. Everything will then regenerate
               </div>
               </div>

               <div class="question">
               <strong>Can you have multiple Given/When/Then attributes attached to a single method in your step definitions class? </strong>
               <div class="answer">
               Yes, you can. This is especially useful to have slightly different formulations for the same automation.
               You can see an example <a href="https://docs.specflow.org/projects/specflow/en/latest/Bindings/Step-Definitions.html#supported-step-definition-attributes" target="_blank" rel="noopener noreferrer">here</a>

               </div>
               </div>

               <div class="question">
               <strong>If the step definitions are global, what does that mean for private state in the step definition classes, setup/mocking in BeforeScenario bound methods, etc.?</strong>
               <div class="answer">
               Every Scenario that gets executed has its own instances of step definition classes.
               A step definition class and all its fields and members are alive and in memory as long as the Scenario in which they were used is executed. After a scenario ended, they are released and not used anymore

               </div>
               </div>

               <div class="question">
               <strong>Is there a limit for the column numbers in a table?</strong>
               <div class="answer">
               No, there is no limit as long as you are not using anonymous tuples. If you are using these, you are limited to 7 columns.
               </div>
               </div>

               <div class="question">
               <strong>What are the advantages of using a custom class over the FeatureContext in context injection?</strong>
               <div class="answer">
               A custom class gives you type-safe access to your data. If you are using the Feature/ScenarioContext, you always need the correct string key and then cast to the right datatype to get to your data. This can be error-prone.
               </div>
               </div>

               <div class="question">
               <strong>How can I use CreateSet for a complex data model?</strong>
               <div class="answer">
               This is not possible. If you get into this need, we suggest rechecking the Formulation of your table if all columns are essential.
               If it is, we recommend in as a first step to use CreateSet to convert a row of the table to a POCO for the row, and as the second step, convert the POCO to your entities/classes

               </div>
               </div>

               <div class="question">
               <strong>How do I share step definitions between multiple projects?</strong>
               <div class="answer">
               You can configure in the specflow.json file in which assemblies SpecFlow should look for step definitions. More details are <a href="https://docs.specflow.org/projects/specflow/en/latest/Bindings/Use-Bindings-from-External-Assemblies.html" target="_blank" rel="noopener noreferrer">here</a>
               </div>
               </div>

               <div class="question">
               <strong>How do I write some messages to the test output?</strong>
               <div class="answer">
               Since SpecFlow 3.8, there is a dedicated API for writing messages to output regardless of which unit test runner you are using.It is called ISpecFlowOutputHelper, more information <a href="https://docs.specflow.org/projects/specflow/en/latest/outputapi/outputapi.html" target="_blank" rel="noopener noreferrer">here</a>
               </div>
               </div>

               <div class="question">
               <strong>How do I initialize a Selenium WebDriver for a whole Feature?</strong>
               <div class="answer">
               One way to do it is this:
               <pre>
               [Binding]
               public class SpecflowHooks
               {
                   private static IWebDriver driver;
                   private readonly IObjectContainer container;
               
                   public SpecflowHooks(IObjectContainer container)
                   {
                       this.container = container;
                   }
               
                   [BeforeFeature]
                   public static void OneTime()
                   {
                       driver = new ChromeDriver(…); 
                   }
               
                   [BeforeScenario]
                   public void SetUp()
                   {
                       container.RegisterInstanceAs<IWebDriver>(driver);
                   }
               
                   [AfterScenario]
                   public void TearDown()
                   {
                   }
               
                   [AfterFeature]
                   public static void FeatureTearDown()
                   {
                       if (driver == null)
                           return;
               
                       driver.Close();
                       driver.Dispose();
                       driver = null;
                   }
               }               
               </pre>
               </div>
               </div>

               <div class="question">
               <strong>What is the difference between the Before/After- Scenario and the Before/After- ScenarioBlock Hooks?</strong>
               <div class="answer">
               The current ScenarioBlock changes when you switch from one step type (Given/When/Then) to another. The hooks are called when this happens.
               </div>
               </div>

               <div class="question">
               <strong>How can I retry a failed Scenario?</strong>
               <div class="answer">
               The easiest way is to use the SpecFlow+ Runner. It has a built-in retry functionality. You can find the documentation at <a href="https://docs.specflow.org/projects/specflow-runner/en/latest/Profile/Execution.html#retryfor" target="_blank" rel="noopener noreferrer">here</a>.
               </div>
               </div>

               <div class="question">
               <strong>Is it possible to mark a step as failed and carry on running the test?</strong>
               <div class="answer">
               No, this is not possible.
               </div>
               </div>

               <div class="question">
               <strong>How can I skip/ignore scenarios at runtime?</strong>
               <div class="answer">
               You need at least SpecFlow 3.1 to do it.

                    <pre>
                    [Binding]
                  public sealed class StepDefinitions
                  {
                     private readonly IUnitTestRuntimeProvider _unitTestRuntimeProvider;

                     public CalculatorStepDefinitions(IUnitTestRuntimeProvider unitTestRuntimeProvider)
                     {
                           _unitTestRuntimeProvider = unitTestRuntimeProvider;
                     }

                     [When("your binding")]
                     public void YourBindingMethod()
                     {
                           _unitTestRuntimeProvider.TestIgnore("This scenario is always skipped");
                     }
                  }
                  </pre>  


               </div>
               </div>

               <div class="question">
               <strong>How can I switch test runner?</strong>
               <div class="answer">
               You need to switch the NuGet package that configures the test runner in your project. You find the list of them <a href="https://docs.specflow.org/projects/specflow/en/latest/Installation/Unit-Test-Providers.html" target="_blank" rel="noopener noreferrer">here</a>
               </div>
               </div>

               <div class="question">
               <strong>Is it possible to mark a step as failed and carry on running the test?</strong>
               <div class="answer">
               No, this is not possible.
               </div>
               </div>

               </div>
            </section>
            <section>
               <h3>SpecFlow+ Excel</h3>
               <div class="questions">

               <div class="question">
               <strong>When will SpecFlow+ Excel be available for SpecFlow 3?</strong>
               <div class="answer">
               We do not currently have a schedule for .NET Core support for SpecFlow+ Excel
               </div>
               </div>
               </div>
            </section>

         <section>
            <h3>SpecFlow+ Runner</h3>
            <div class="questions">

            <div class="question">
            <strong>What are the advantages of SpecFlow+ Runner?</strong>
            <div class="answer">
            Some of the key features of SpecFlow+ Runner are:

            <ul>
             <li> Support for multiple <a href="https://specflow.org/plus/documentation/targets/" target="_blank" rel="noopener noreferrer">targets</a>, allowing you to write a single test to target different environments (e.g. x86 and x64, various browsers).</li>
             <li> <a href="https://specflow.org/plus/documentation/DeploymentTransformation/" target="_blank" rel="noopener noreferrer">Configuration file transformations</a>, which can also be used in conjunction with targets. This allows you to transform your configuration file for different platforms or web browsers, or set up a separate database instance for each thread using <a href="https://specflow.org/plus/documentation/placeholders/" target="_blank" rel="noopener noreferrer">placeholders</a></li>
             <li> Advanced reporting options using CSHTML templates. You can configure the output to meet your specific needs, both by customizing the formatting and determining which data to include and how it should be laid out. 3 default templates are included to get you started that output your test reports as either HTML, JSON or XML.</li>
             <li> Adaptive test scheduling mode priorities previously failing tests over stable tests based on your execution history. Note that this feature requires you to set up a SpecFlow+ Runner server.</li>
             <li> <a href="https://docs.specflow.org/projects/specflow/en/latest/Execution/Parallel-Execution.html" target="_blank" rel="noopener noreferrer">Parallelisation</a> and isolation options for multi-threaded test execution. You can isolate threads by AppDomain, SharedAppDomain or Process.</li>
            
            </ul>
               </div>
            </div>

            <div class="question">
               <strong>I have already activated a SpecFlow account, but the SpecFlow+Runner is still asking me to sign up</strong>
               <div class="answer">
               
               1. Add the following system environment variable in windows

               Variable name: SPECFLOW_PLUS_USE_PROXY_CREDENTIALS
               
               Variable value: 1<br></br>                             
               
               1. Restart the application
               If you run the tests with Visual Studio please restart your Visual Studio (exit, open again).
               This is necessary to pick up the new environment variable setting.<br></br>
               
               1. Run the SpecFlow+Runner tests again
               </div>
               </div>
 
               <div class="question">
               <strong>I am getting a proxy error after signing up for a SpecFlow account, what should I do?</strong>
               <div class="answer">
               To resolve this issue:

               1. Add the following system environment variable in windows
               
               Variable name: SPECFLOW_PLUS_USE_PROXY_CREDENTIALS
               
               Variable value: 1 <br></br>
               
                
               
               1. Restart the application
               If you run the tests with Visual Studio please restart your Visual Studio (exit, open again).
               This is necessary to pick up the new environment variable setting.<br></br>
               
               1. Run the SpecFlow+Runner tests again<br></br>
               </div>
               </div>

               <div class="question">
               <strong>Issue due to having multiple solutions with different versions of SpecFlow+ installed</strong>
               <div class="answer">
               When loading a solution containing SpecFlow+, Visual Studio caches the SpecFlow+ components. If you open a new solution containing a SpecFlow+ project, Visual Studio will retain the cached version of the SpecFlow+ components in memory. If the version used by the two projects is different, this means that there will be a version mismatch.

               You can avoid this issue by either upgrading all your solutions to the same version of SpecFlow+, or by restarting Visual Studio to flush the cache before opening the new solution.
               </div>
               </div>

               <div class="question">
               <strong>Tests are not displayed in the Test Explorer window when using SpecFlow+ Runner</strong>
               <div class="answer">
               Note: As of Visual Studio 2017 15.7 the temporary files are no longer used. The following only applies to earlier versions of Visual Studio.

               The Visual Studio Test Adapter cache may also get corrupted, causing tests to not be displayed. If this happens, try clearing your cache as follows:
               
               1. Close all Visual Studio instances<br></br>
               2. Navigate to your %TEMP%\VisualStudioTestExplorerExtensions\ folder and delete any sub-folders related to SpecFlow/SpecRun, i.e. that have "SpecFlow" or "SpecRun" in their name.<br></br>
               3. Reopen your solution and ensure that it builds.<br></br>
               </div>
               </div>

               <div class="question">
               <strong>Visual Studio 2015: Tests are not displayed in the Test Explorer window when using SpecFlow+ Runner</strong>
               <div class="answer">
               Visual Studio 2015 handles solution-level NuGet packages differently (those registered in the <i>.nuget\packages.config</i> file of the solution). As a result, solution-level NuGet packages must be listed in the projects that use them, otherwise Test Explorer cannot recognise the test runner.

               To fix this issue, either re-install the SpecFlow+ Runner NuGet packages, or add the dependency on the SpecRun.Runner package (<i> package id="SpecRun.Runner" version="1.2.0" </i>) to the packages.config file of your SpecFlow projects. You might need to restart Visual Studio to see your tests.
                
               </div>
               </div>
            </div>
            </section>



      <section>
      <h3>SpecFlow Gherkin Editor</h3>
      <div class="questions">

      <div class="question">
      <strong>Why should I use the Gherkin Editor?</strong>
      <div class="answer">
      The Gherkin Editor enables you to quickly collaborate, draft and share Gherkin feature files with your team and business stakeholder. The editor allows organizing all your Gherkin feature file drafts in just one place and simplifies the collaboration with your non-technical team members and business stakeholders. 
      </div>
      </div>
      
      <div class="question">
      <strong>How can I create an account for the Gherkin Editor?</strong>
      <div class="answer">
      You can create an account by clicking on Create an account on the top right corner of the editor and sign in with your Microsoft account. If you don't have a Microsoft account yet, you are able to create one for free during the sign-in process.

      In case you use a corporate or student account and run into admin consent issues, please use your personal account instead or send <a href="https://docs.specflow.org/en/latest/adminconsent.html" target="_blank" rel="noopener noreferrer">this link</a> to your admin to grant you access. 
      </div>
      </div>

      <div class="question">
      <strong>Can I use my existing SpecFlow account for the Gherkin Editor?</strong>
      <div class="answer">
      Yes, only one SpecFlow account is required to use all our SpecFlow+ products. Simply click on Sign In on the top right corner of the Gherkin Editor and use the same Microsoft account you used for other SpecFlow+ products
      </div>
      </div>

      <div class="question">
      <strong>How can I store a feature file online?</strong>
      <div class="answer">      
      You can save and store feature files associated with your SpecFlow account by clicking the Sign in to save button on the top right of the Gherkin Editor.
      </div>
      </div>
      
      <div class="question">
      <strong>How can I share my feature files in the Gherkin Editor?</strong>
      <div class="answer">      
      You can share your feature files by clicking the Share button on the top right corner of the Gherkin Editor. Please note this is only available to users who have created a free account and are signed in.

      In general, you can choose between three access levels: 
      
      1. "Only me" ~ only you can view and edit the feature file with this link.<br></br>
      2. "Anyone with the link" ~  anyone with the link can view and edit the feature file.<br></br>
      3. "Anyone with the link - read only" ~ anyone with the link can only view the feature file.<br></br>


      </div>
      </div>

      <div class="question">
      <strong>Is the Gherkin Editor free to use?</strong>
      <div class="answer">      
      Yes, the Gherkin Editor is free to use and doesn't require an account sign-up. Only for saving and sharing feature files, a free account sign-up is required.

      </div>
      </div>

      <div class="question">
      <strong>How can I upload an existing feature file?</strong>
      <div class="answer">      
      There is no upload feature in the Gherkin Editor yet. The simplest way to get your existing feature files into the Gherkin Editor is to manually copy/paste them into the editor view and then save them.

      </div>
      </div>

      <div class="question">
      <strong>How can I delete my feature files?</strong>
      <div class="answer">      
      Click on the Feature Files button at the top of the Gherkin Editor to view all your feature files. From here you can delete, download and view the access level for each feature file.
      </div>
      </div>

      <div class="question">
      <strong>What is a Gherkin Editor?</strong>
      <div class="answer">      
      In general, a Gherkin Editor is a text editor that allows you to write feature files using <a href="https://specflow.org/learn/gherkin/" target="_blank" rel="noopener noreferrer">Gherkin syntax</a>.

      Gherkin is a "Business Readable" language created especially for behavior descriptions. Its simplicity allows non-technical users to write specifications and it also allows you to remove logic details from behavior tests. Gherkin serves two purposes: serving as your project's specification/documentation and automated tests.
      
      The SpecFlow Gherkin Editor gives you additional tools to assist you in writing better Gherkin and also gives you the ability to share Gherkin feature files so you can collaborate with your team more easily.
      </div>
      </div>

       </div>
      </section>     

      <section>
      <h3>SpecFlow+ LivingDoc</h3>
      <div class="questions">

      <div class="question">
      <strong>What is SpecFlow+LivingDoc?</strong>
      <div class="answer">
      SpecFlow+LivingDoc is a set of tools that allows you to share and collaborate on Gherkin Feature Files with stakeholders who may not be familiar with developer tools. There are two ways to produce living documentation depending on how you want to use and share it. You have the option to use the Azure DevOps extension which helps you build living documentation in Azure DevOps environment or use the LivingDoc Generator which is a stand-alone generator with no external dependencies. 

      Please check the <a href="https://docs.specflow.org/projects/specflow-livingdoc/en/latest/" target="_blank" rel="noopener noreferrer">documentation page </a>for more info.
      </div>
      </div>

      <div class="question">
      <strong>How can I share the generated living documentation?</strong>
      <div class="answer">
      If you generated your LivingDoc using the <a href="https://docs.specflow.org/projects/specflow-livingdoc/en/latest/LivingDocGenerator/Generating-Documentation.html" target="_blank" rel="noopener noreferrer">CLI tool </a>, the output file will be an HTML file with no external dependencies, therefore you can share this HTML file as you wish. Please check our <a href="https://docs.specflow.org/projects/specflow-livingdoc/en/latest/LivingDocGenerator/sharing-and-publishing.html" target="_blank" rel="noopener noreferrer">documentation page </a> for a few ideas on how to share LivingDoc.
      </div>
      </div>

      <div class="question">
      <strong>What’s the difference between SpecFlow+ LivingDoc Generator and the SpecFlow+ LivingDoc Azure DevOps extension?</strong>
      <div class="answer">
      The LivingDoc Azure DevOps extension integrates into the Azure DevOps environment and allows you to build, view, and share LivingDoc. The LivingDoc Generator on the other hand, is a stand-alone LivingDoc generator with no external dependencies, it allows you to generate LivingDoc HTML files that are not tied to particular environment. Please check our <a href="https://docs.specflow.org/projects/specflow-livingdoc/en/latest/" target="_blank" rel="noopener noreferrer">documentation </a> to learn more.
      </div>
      </div>

      <div class="question">
      <strong>Do I need to use Microsoft Azure DevOps to generate LivingDoc?</strong>
      <div class="answer">
      You can generate living documentation by using the <a href="https://docs.specflow.org/projects/specflow-livingdoc/en/latest/LivingDocGenerator/Generating-Documentation.html" target="_blank" rel="noopener noreferrer">CLI tool </a> which is a stand-alone product with no external dependencies. You can find all the information you need regarding how to create, and use LivingDoc <a href="https://docs.specflow.org/projects/specflow-livingdoc/en/latest/index.html" target="_blank" rel="noopener noreferrer">here</a>.
      </div>
      </div>

      <div class="question">
      <strong>My JSON file name is FeatureData.json instead of TestExecution.json, what should I do?</strong>
      <div class="answer">      
      This indicates that you are using an older version of SpecFlow+LivingDoc. Please check our migration guide <a href="https://docs.specflow.org/projects/specflow-livingdoc/en/latest/Guides/Generator-Migration-v3.4-v3.5.html" target="_blank" rel="noopener noreferrer">here </a> to upgrade to the latest version.
      </div>
      </div>
   </div>
   </section> 

   <section>
      <h3>SpecMap</h3>
      <div class="questions">

      <div class="question">
      <strong>List of known issues</strong>
      <div class="answer">
      <ul>
      <li>It is not possible to drag & drop items from the backlog query to the map in TFS when using Edge.</li>

      <li>Issues can arise when using templates in languages other than English. This may also result in an empty default query. You can however define your own queries and use these instead.</li>
      
      <li>SpecMap requires certain fields to be present in your template; if the fields are missing, errors will occur. This means that custom templates are not currently supported.</li>
      
      <li>Synchronization issues can occur in setups with high latency, e.g. where the server is in a different country from the users. This is more likely to occur using the on-premise (TFS) extension. Please open a support request if you are experiencing long delays, particularly when receiving messages that the map has been updated and your changes cannot be saved as a result.</li>
      
      <li>SpecMap is not fully compatible with the new navigation layout in Azure DevOps (VSTS) (currently only available as a preview). The backlog queries are empty when not using the default team. A workaround is to define your own queries.</li>
      <ul>


      </div>
      </div>

      <div class="question">
      <strong>How is SpecMap licensed?</strong>
      <div class="answer">      
      In order to use SpecMap, you need to sign up for a free personal SpecFlow account. SpecMap is free of charge and will remain free forever.
      </div>
      </div>

      <div class="question">
      <strong>Is it possible to restrict access to specific maps per user?</strong>
      <div class="answer">      
      Access to projects and work items is determine by a user’s TFS project/work item permissions. Users without permission to access a project cannot access the maps in that project. If a user has access to a project, but not to certain work items, the user can browse the maps, but will not see the details (title, etc) of the mapped work items they are not permitted to access.

      There is currently no means of restricting access to a particular map outside of these options. We intend to add access settings for maps in the future, allowing you to grant read-only access or deny access to specific maps.
      </div>
      </div>
     
      <div class="question">
      <strong>Is it possible to use custom TFS templates with SpecMap?</strong>
      <div class="answer">      
      Since January, 2020 SpecMap is free forever.

      To properly list SpecMap as a free extension in the Azure DevOps marketplace we've changed the configuration of the extension and removed the Paid flag in version 0.5.109.
      
      This configuration change of the flags is not automatically applied when SpecMap is installed on an on-premise Azure Devops Server (formerly Team Foundation Server).
      
      Users using any SpecMap version prior to 0.5.109 will see the following an error message
      
      In order to fix this issue the Flags value of the extension has to be manually updated in the Azure Devops Database, using the following steps:
      
      1. Connect to the Azure Devops Server Configuration Database<br></br>
      2. Create a backup before making any changes<br></br>
      3. Locate the [Gallery].[tbl_Extension] table<br></br>
      4. Locate the row with the [ExtensionName] "SpecMap"<br></br>
      5. Update the value of the [Flags] from 276 (Public, Paid, Validated) to 260 (Public, Validated)<br></br>
      6. Attempt to update again SpecMap which should succeed now <br></br>


      </div>
      </div>

      <div class="question">
      <strong>Are external network connections required for SpecMap on TFS ("offline")?</strong>
      <div class="answer">      
      SpecMap only communicates with the server where the extension is installed. This is either Azure Devops or the on-premise TFS server where it is hosted.

      All data is stored on this server, and SpecMap does not send nor store data elsewhere.
      
      External network connections are only used by the monitoring functions, which connect to an external Azure AppInsights service. However, this is not required for SpecMap to function. We only collect information on users/and usage, which can help us troubleshoot issues with SpecMap.
      </div>
      </div>
   </div>
   </section> 

   <section>
      <h3>SpecFlow Account</h3>
      <div class="questions">

      <div class="question">
      <strong>Can I use other platforms than Microsoft to sign up for a SpecFlow account?</strong>
      <div class="answer">      
      Microsoft is the only supported platform to use to sign-up for a SpecFlow account. But, we are considering other options at the moment and there is a <a href="https://support.specflow.org/hc/en-us/community/posts/360014469817--SpecFlow-Account-Sign-up-for-SpecFlow-account-using-GitHub" target="_blank" rel="noopener noreferrer">feature request </a> for it.

      </div>
      </div>

      <div class="question">
      <strong>How do I sign out/deactivate a SpecFlow account?</strong>
      <div class="answer">      
      We currently do not have this feature in our product range. Please reach out to support <a href="https://support.specflow.org/agent/dashboard" target="_blank" rel="noopener noreferrer">here</a> and we will take care of it for you. 

      </div>
      </div>

      <div class="question">
      <strong>Where is the user data for the SpecFlow account stored?</strong>
      <div class="answer">      
      The user data is stored in Azure, in the West Europe data center region (Netherlands, EU), you can read more information <a href="https://azure.microsoft.com/en-us/global-infrastructure/data-residency/" target="_blank" rel="noopener noreferrer">here</a>
           
      </div>
      </div>

      <div class="question">
      <strong>Where can I find your privacy policy?</strong>
      <div class="answer">      
      Our privacy policy can be found <a href="https://specflow.org/privacy-policy/" target="_blank" rel="noopener noreferrer">here</a>.
           
      </div>
      </div>

      <div class="question">
      <strong>How can I delete my SpecFlow account?</strong>
      <div class="answer">      
      If you would like to delete your SpecFlow account, please open a <a href="https://support.specflow.org/hc/en-us/requests/new" target="_blank" rel="noopener noreferrer">support request</a>.

      Note that deleting your account will prevent you from using any of the licensed products (SpecFlow+ Runner, SpecFlow+ LivingDoc, SpecMap). Deleting your account will not affect any data stored locally in Azure DevOps. 
      Even after your account is deleted, you will still see the SpecFlow+ LivingDoc and SpecMap entries in Azure DevOps. To remove these entries, you need to uninstall the extensions. This will also remove any data specific to the extension (i.e. your maps in SpecMap and your living documentation in SpecFlow+ LivingDoc).
           
           
      </div>
      </div>

      <div class="question">
      <strong>Do I need to sign-up for a SpecFlow account if I have an existing valid license key?</strong>
      <div class="answer">      

      No, you don't need to do anything right now. Only once the license keys expire each of your team members will be asked to create a free personal SpecFlow account.

      </div>
      </div>

      <div class="question">
      <strong>What if I am working in an offline environment?</strong>
      <div class="answer">      

      If you are working in an offline environment, please open a <a href="https://support.specflow.org/hc/en-us/requests/new" target="_blank" rel="noopener noreferrer">support request</a>. You will receive information on how to license your software without an internet connection. We intend to provide an offline licensing method in the future to cater to this need
      
      </div>
      </div>

      <div class="question">
      <strong>Do I need to create a SpecFlow account to use SpecFlow+ Runner on a build server</strong>
      <div class="answer">      

      SpecFlow+ Runner recognizes the most popular build servers and does not require a product activation when running in build server mode. If you encounter problems with running your tests on a build server please open a <a href="https://support.specflow.org/hc/en-us/requests/new" target="_blank" rel="noopener noreferrer">support request</a> with the details of your build server.
      
      </div>
      </div>

      <div class="question">
      <strong>How can I sign up for a free SpecFlow account?</strong>
      <div class="answer">      

      The first time you use one of our products, you will be asked to sign in with your Microsoft account and set up your SpecFlow account. Once you have set up your free SpecFlow account, you can use it to sign in all SpecFlow+ products. Learn more about the sign up <a href="https://specflow.org/2020/introducing-the-specflow-account/" target="_blank" rel="noopener noreferrer">here</a>.

      </div>
      </div>  

   </div>
   </section> 




         </div>
      </div>
      <script type="text/javascript">
         window.addEventListener("DOMContentLoaded", function() {
            const groups = [];
            document.querySelectorAll("#faq-sections section").forEach(section => {
               const heading = section.querySelector("h3");
               if (!heading) {
                  return;
               }
               heading.addEventListener("click", () => {
                  section.classList.toggle("open");
               });
               const questions = [];
               section.querySelectorAll(".questions .question").forEach(q => {
                  try {
                     questions.push({
                        question: q.querySelector("strong").textContent.toLocaleLowerCase(),
                        answer: q.querySelector(".answer").textContent.toLocaleLowerCase(),
                        element: q
                     });
                     q.querySelector("strong").addEventListener("click", function() {
                        q.classList.toggle("open");
                     })
                  } catch (e) {
                     console.error(e);
                  }
               });
               groups.push({
                  name: heading.textContent,
                  questions: questions,
                  element: section
               })
            });

            const filterInput = document.getElementById("filter");
            const groupSelect = document.getElementById("group-select");

            const o = document.createElement("option");
            o.value = o.text = "All";
            groupSelect.add(o);
            groups.forEach(group => {
               const o = document.createElement("option");
               o.value = o.text = group.name;
               groupSelect.add(o);
            });

            const filter = () => {
               const searchTerm = filterInput.value.toLocaleLowerCase();
               groups.forEach(group => {
                  let count = 0;
                  if (group.name === groupSelect.value || groupSelect.value === "All") {
                     group.questions.forEach(question => {
                        question.element.classList.remove("open");
                        if (question.question.includes(searchTerm) || question.answer.includes(searchTerm)) {
                           count++;
                           question.element.style.display = "block";
                        } else {
                           question.element.style.display = "none";
                        }
                     })
                  }
                  if (count) {
                     group.element.style.display = "block";
                  }  else {
                     group.element.style.display = "none";
                  }
               })
            }

            groupSelect.addEventListener("change", filter)
            let timeout;
            filterInput.addEventListener("keyup", () => {
               clearTimeout(timeout);
               timeout = setTimeout(filter, 100)
            });
         });
      </script>
   </embed>