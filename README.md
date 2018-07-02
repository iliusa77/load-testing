# Load-testing

## Taurus

Tested on Ubuntu 14

preparation:
   <pre>sudo add-apt-repository ppa:tsung/stable -y</pre>
   <pre>sudo add-apt-repository ppa:webupd8team/java -y</pre>
   <pre>sudo apt update</pre>
   <pre>sudo apt install -y unzip curl libxml2-dev libxslt-dev python3-dev python3-pip python-virtualenv apache2-utils siege tsung oracle-java8-installer oracle-java8-set-default</pre>
   <pre>cd Taurus</pre>
   <pre>virtualenv -p python3 .venv</pre>
   <pre>source .venv/bin/activate</pre>
   <pre>pip3 install -r requirements.txt</pre>

run test on jmeter executor:
   <pre>bzt bzt_jmeter_test.yml</pre>

run test on tsung executor:
   <pre>bzt bzt_tsung_test.yml</pre>

run test on apache benchmark executor:
   <pre>bzt bzt_ab_test.yml</pre>

run test on siege executor:
   <pre>bzt bzt_siege_test.yml</pre>



## SmartMeter

Tested on Ubuntu 14

preparation:
   <pre>cd SmartMeter</pre>
   <pre>curl -o SmartMeter_1.7.0_linux.zip http://smartmeter-api.etnetera.cz/download/release/1.7.0/linux/full/SmartMeter_1.7.0_linux.zip</pre>
   <pre>unzip SmartMeter_1.7.0_linux.zip && rm -rf SmartMeter_1.7.0_linux.zip</pre>
