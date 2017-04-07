## Workshop-Array
### study 01
#### merge array
```php
 $users = ['Asep Dadang Supriadi', 'Akmal Fuady', 'Yandi Fitriyanto'];

 $users_new = ['Ricky Andika Putra', 'Ramadani'];

 $result = array_merge($users, $users_new);

 print_r($result);

```

### case study 3
#### remove last values in array
```php
$users = ['Ricky Andika Putra', 'Ramadani', 'Asep Dadang Supriadi', 'Akmal Fuady', 'Yandi Fitriyanto'];

array_pop($users);
```

### case 4
#### remove first values in array

```php
$users = ['Ricky Andika Putra', 'Ramadani', 'Asep Dadang Supriadi', 'Akmal Fuady', 'Yandi Fitriyanto'];

array_shift($users);
print_r($users);
```

### case 5
#### show unique array from 2 merge array

```php
$input_one = ['Ricky Andika Putra', 'Ramadani', 'Asep Dadang Supriadi', 'Akmal Fuady', 'Yandi Fitriyanto'];
$input_two = ['Ricky Andika Putra', 'Yandi Fitriyanto', 'Muhammad Sholeh', 'Yadi Cahyadi'];

$merge = array_merge($input_one, $input_two);

$result = array_unique($merge);

print_r($result);
```

### case 6
#### show diff values array

```php
$input_one = ['Ricky Andika Putra', 'Ramadani', 'Asep Dadang Supriadi', 'Akmal Fuady', 'Yandi Fitriyanto'];
$input_two = ['Ricky Andika Putra', 'Yandi Fitriyanto', 'Muhammad Sholeh', 'Yadi Cahyadi'];

$result = array_diff($input_one, $input_two);
print_r($result);
```

### case study 7
#### show intersect values from 2 array

```php
$input_one = ['Ricky Andika Putra', 'Ramadani', 'Asep Dadang Supriadi', 'Akmal Fuady', 'Yandi Fitriyanto'];
$input_two = ['Ricky Andika Putra', 'Yandi Fitriyanto', 'Muhammad Sholeh', 'Yadi Cahyadi'];

$result = array_intersect($input_one, $input_two);
print_r($result);
```

### case study 8
#### get array_keys

```php
$users = [
'user1@example.com' => 'Adimas Lutfi Wicaksono',
'user2@example.com' => 'Salman Alfarisi',
'user3@example.com' => 'Muhammad Sholeh',
'user4@example.com' => 'Yadi Cahyadi',
'user5@example.com' => 'Maya Maulani',
];
$email = array_keys($users);
print_r($email);
```

### case study 9
#### get array_values

```php
$users = [
'user1@example.com' => 'Adimas Lutfi Wicaksono',
'user2@example.com' => 'Salman Alfarisi',
'user3@example.com' => 'Muhammad Sholeh',
'user4@example.com' => 'Yadi Cahyadi',
'user5@example.com' => 'Maya Maulani',
];

print_r(array_values($users));
```

### case study 10
#### get unique array / not duplicate

```php
$names = [
'Adimas Lutfi Wicaksono', 'Salman Alfarisi', 'Adimas Lutfi Wicaksono',
'Muhammad Sholeh', 'Yadi Cahyadi', 'Maya Maulani', 'Maya Maulani'
];

print_r(array_unique($names));
```

### case study 11
#### return values from multidimensional array

```php
  $users = [
    [
      'id'     => 1,
      'name'   => 'Adimas Lutfi Wicaksono',
    ],
    [
      'id'     => 2,
      'name'   => 'Salman Alfarisi',
    ],
    [
      'id'     => 3,
      'name'   => 'Muhammad Sholeh',
    ],
    [
      'id'     => 4,
      'name'   => 'Yadi Cahyadi',
    ],
    [
      'id'     => 5,
      'name'   => 'Maya Maulani',
    ],
];

$names = [];

foreach ($users as $key => $value) {
    $names[$key] = $value['name'];
}

print_r($names);
```

### case study 12
#### return array after change specific values

```php
$users = [
  [
    'id'     => 1,
    'name'   => 'Adimas Lutfi Wicaksono',
    'gender' => 1,
  ],
  [
    'id'     => 2,
    'name'   => 'Salman Alfarisi',
    'gender' => 1,
  ],
  [
    'id'     => 3,
    'name'   => 'Muhammad Sholeh',
    'gender' => 1,
  ],
  [
    'id'     => 4,
    'name'   => 'Yadi Cahyadi',
    'gender' => 1,
  ],
  [
    'id'     => 5,
    'name'   => 'Maya Maulani',
    'gender' => 2,
  ],
];


foreach ($users as $key => $user) {
    if ($users[$key]['gender'] == 1) {
        $users[$key]['gender'] = 'Male';
    } else {
        $users[$key]['gender'] = 'Female';
    }
}

print_r($users);
```

### case 16
#### push new values into array

```php
$users = ['Asep Dadang Supriadi', 'Akmal Fuady', 'Yandi Fitriyanto'];

$users_new = 'Ricky Andika Putra';
array_push($users, $users_new);

print_r($users);
```

### case study 17
#### set new values in first index

```php
$users = ['Asep Dadang Supriadi', 'Akmal Fuady', 'Yandi Fitriyanto'];

$users_new = 'Ricky Andika Putra';
array_unshift($users, $users_new);

print_r($users);
```
