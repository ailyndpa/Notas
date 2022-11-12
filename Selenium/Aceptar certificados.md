Aceptar certificados
========================

**Para chrome:**
ChromeOptions opt=new ChromeOptions();
opt.setAcceptInsecureCerts(true);
WebDriver driver=new ChromeDriver(opt);

**Para Firefox:**
FirefoxOptions option= new FirefoxOptions();		
option.setAcceptInsecureCerts(true);
WebDriver driver = new FirefoxDriver(option);

**Para Edge:**
EdgeOptions option= new EdgeOptions();		
option.setAcceptInsecureCerts(true);
WebDriver driver = new EdgeDriver(option);