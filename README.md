# Load-testing

## Taurus

Tested on Ubuntu 14

preparation:
   <pre>sudo apt update</pre>
   <pre>sudo apt install -y libxml2-dev libxslt-dev python3-dev python3-pip python-virtualenv apache2-utils siege tsung</pre>
   <pre>cd Taurus</pre>
   <pre>virtualenv -p python3 .venv</pre>
   <pre>source .venv/bin/activate</pre>
   <pre>pip3 install -r requirements.txt</pre>

run test on jmeter executor:
   <pre>bzt bzt_jmeter_test.yml</pre>

run test on tung executor:
   <pre>bzt bzt_tsung_test.yml</pre>

