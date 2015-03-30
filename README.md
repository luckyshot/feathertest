# FeatherTest
## Automated Website Testing for Google Chrome

FeatherTest is a free Google Chrome extension to serve as a quick way to build simple tests and automate processes, you can also use it to register accounts or fill forms with data. It is really flexible, you can use any JavaScript and jQuery code to write your tests, doesn't need any server setup and once the test is written anyone in the team can run them from their browsers.

Read the full documentation, code examples, notes and more here:
http://xaviesteve.com/5302/feathertest-automated-website-testing-extension-google-chrome

Install the extension here: https://chrome.google.com/webstore/detail/feathertest-website-autom/cpconfnklmionglnfabhmpckegbjdbfe

### Test example

<pre>'feathertest'
// go to the homepage
location.href = '/'

// search for 'speakers'
$('#q').val( 'speakers' )
$('#form').submit()

// wait one second
1000

// check results are showing
ft.isTrue( $('li.results .item').length )</pre>

### Changelog

#### 1.0.5

- Including info on each assertion
- Removed unnecessary <code>function(){return}</code> from <code>ft.isTrue()</code> documentation
- Improved console coloring for better readability

#### 1.0.4

- <code>ft.set()</code> and <code>ft.get()</code> methods to save custom variables
- Removed extra <code>console.log</code> and less <code>console.info</code> icons for better readability
- Fixed bug when canceling test prompt would try to run it anyway (2)
- Code quality run

#### 1.0.3

- Fixed bug when canceling test prompt would try to run it anyway

#### 1.0.2

- Prefixed 'url' localStorage variable to 'ft_url' to avoid any possible conflicts with other variable definitions

#### 1.0.1

- First commit
