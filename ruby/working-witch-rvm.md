To install RVM simply use creppin' curl :stuck_out_tongue_closed_eyes:.
```bash
$ curl -L get.rvm.io | bash -s stable
```

To update RVM
```bash
$ rvm get stable
```

Check known rubies
```bash
$ rvm list known
```

To install specific ruby version:
```bash
$ rvm install 2.2.2
```

To list rubies
```bash
$ rvm list
```

Select rubies
```bash
# system ruby
$ rvm use system
# ruby 2.2.2 installed before
$ rvm use ruby-2.2.2
# set chosen ruby as default
$ rvm use --default ruby-2.2.2
```

Working with gamesets.
To list gamesets
```bash
$ rvm list gemsets
$ rvm gemset list
```

To create gemset and use it
```bash
$ rvm gemset create gameset_name
$ rvm gemset use gameset_name
$ rvm use ruby-2.2.2@gemset_name
```

