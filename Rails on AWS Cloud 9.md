CONTENTS OF THIS FILE
---------------------
 
 * Introduction
 * Requirements
 * Installation
 * Troubleshooting
 * FAQ
 
 
 INTRODUCTION
 ------------
 
 Installing Rails Apps seems to be a hassle for many of us. Whether you are using a PC or if your Mac isn't working, Amazon Web Services' Cloud 9 provides an alternative that is user-friendly and easy to install. 
 There are still some challenges that you need to face in order to successfully run your Rails App, but hopefully, this guide is able to help you!
 
 REQUIREMENTS
 ------------
 * Have access to Amazon Web Services and Cloud 9. 
 * Save this command for later: \curl -sSL https://raw.githubusercontent.com/LEARNAcademy/cloud9-config/master/setup.sh | bash -s
 
 INSTALLATION
 ------------
Follow the instructions below and go down them step-by-step:
 
 * Create your IDE using Cloud 9. Name it whatever you want. 
 
 * $ rails new (your-app-name) -d postgresql -T
 
 * $ gem install pg -v 0.21.0
 
 * You might not need this step but in case you get an error here, use the following line of code: bundle exec spring binstub -all
 
 * cd (your-app-name)
 
 * Run this curl command provided by Sarah: \curl -sSL https://raw.githubusercontent.com/LEARNAcademy/cloud9-config/master/setup.sh | bash -s
 
 * bundle install
 
 * rails db:create
 
 * Generate your model: $ rails generate model (Example) (attribute1:datatype)...(attribute(n):datatype(n))
 
 * rails db:migrate
 
 * rails generate controller main
 
 * rails c (if you want to add more entries into your database! If not, just ignore this part/ come back to it later)
 
 * bundle install
 
 * rails s
 
 * Click Preview (this button is located at the top of the screen above the coding IDE next to the green Run button)
 
 * Under Preview click 'Preview Running Application' 
    - This will cause a window to open in the same browser. COPY the error message that is displayed in the body of that page. 
 
 * In the folder config find the file application.rb
 
 * COPY the error message from the window into the Module <app-name> in the class Application Body < Rails::Application
 
 * SAVE and return to the terminal. 
 
 * Run the $ rails S command again and click the Preview App button. This time, open the preview in a new tab instead of in the IDE. Please see the screenshot provided.
 
 * You will have the Rails landing page!
 
 * If you want to play around and do the projects we've done in class, add your 'example_model_here/new....' to the end of the very long amazonaws.com link. 
 
 Please let me know if you have any questions!! I'd be more than happy to help! :) 

 TroubleShooting
 ------------ 
 I will post my history of commands in the terminal for those that are not able to get it. There might be like 100000 instances of something going wrong, so if that happens, just slack me or lets talk after class and I can try and help!

