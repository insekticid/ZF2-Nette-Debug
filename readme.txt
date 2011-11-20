Nette Framework Debug
==========================


Installation
------------

Add Nette namespace to your autoloader

    protected function initAutoloader()
    {
        \Zend\Loader\AutoloaderFactory::factory(array(
            'Zend\Loader\StandardAutoloader' => array(
                'namespaces' => array(
                    'Nette'   =>  __DIR__ . '/../library/Nette'
                ),
            ),
        ));
    }
    
Init Debug in your Zend bootstrap file

	protected function initDebug($env = 'production')
	{
		include_once('Nette\Diagnostics\exceptions.php');

		if ( 'production' !== $env && 'testing' !== $env )
		{
			\Nette\Diagnostics\Debugger::_init();
			\Nette\Diagnostics\Debugger::enable();
			\Nette\Diagnostics\Debugger::$strictMode = 1;
			//Nette\Diagnostics\Debugger::$consoleMode = 1;
		}
	}

Have fun!


-----


Nette Framework is a powerful, component-based and event-driven framework
for creating web applications and services in PHP 5.2 & 5.3. Nette Framework
is designed with simplicity, speed and flexibility in mind. It allows developers
to easy built better websites.

homepage: http://nette.org
repository: http://github.com/nette/nette
