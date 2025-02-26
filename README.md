# ProxiBlue_HyvaGlobalLoading module

Ads a global loading indicator. 

* activates on any form submit to indicate action 
* can be activated, de-activated by setting a global variable ```window.isLoading = true|false```
* listens to any ajax fail/complete events to deactive (prevents hung site with loader never going away)
* Throws an event that you cna listen to if global variable changes so you can do things when loader shows/hides

Uses Hyva default ui/loader.phtml ```Hyva_Theme::ui/loading.phtml```

Customise by placing in your theme ```app/design/frontend/{THEME}/{NAME}/Hyva_Theme/templates/ui/loading.phtml```


## Installation

* add composer repo: ```composer config repositories.github.repo.repman.io composer https://github.repo.repman.io```
* install package using composer ```composer require proxi-blue/module-hyva-global-loading```
* enable module ```./bin/magento module:enable ProxiBlue_HyvaGlobalLoading```
* ```./bin/magento setup:upgrade```
* ```./bin/magento setup:di:compile```

## Note on liability 

Not yet used in a production environment, so you use this at your own risk

