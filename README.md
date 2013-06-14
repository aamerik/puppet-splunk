splunk

This is the splunk module.  It requires Puppet 2.6.2 or later.

Disabled inputs for  sourcetype "lsof" "ps" as they are chatty and create a lot of events

## Pre-Commit Hook
To use the pre-commit hook supplied (taken from another github repo, url to be supplied, link the hook to .git/hooks with this command
ln -s pre-commit.puppet-lint .git/hooks/pre-commit

## Example Usage

### splunk::ulimit
=== Examples

>  splunk::ulimit { 'nofile':
>    value => '16384',
>  }
