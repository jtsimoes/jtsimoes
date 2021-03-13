```php
<?php

namespace jtsimoes;

class About extends Me
{
    const name = 'João Tomás Simões';
    
    public function getJobs(): array
    {
        return [
            'student' => [
                'company' => 'University of Aveiro',
                'course' => 'Computers and Telematics Engineering',
                'startDate' => '1505779200'
            ],
            'web developer' => [
                'company' => 'Agora Aveiro',
                'url' => 'https://agoraaveiro.org/'
            ],
            'photographer' => [
                'company' => '',
                'portfolio' => 'https://www.instagram.com/jtsimoes/'
            ]
        ];
    }

    public function getSkills(): array
    {
        return [
            PHP::class,
            JavaScript::class,
            HTML::class,
            CSS::class,
            SQL::class,
            C++::class,
            Java::class,
            Python::class,
        ];
    }

    private function getGoal(): string
    {
        return 'Finish the university course';
    }
}

echo "Hi there! Welcome to my profile 👋";

?>
```
