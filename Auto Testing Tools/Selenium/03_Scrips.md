## 3. Selenium Scripts

There are three models introduced in section 2. I will focus on the **local model** in this repository using Python programming language and maybe add a simple distributed computing model sample if I can build up a distributed computing testing bed.

### Testing environment verify
```
from selenium.webdriver import Firefox

with Firefox() as driver:
    driver.get("https://selenium.dev")
```

### Browser navigation
```

driver.get("https://selenium.dev")  
```