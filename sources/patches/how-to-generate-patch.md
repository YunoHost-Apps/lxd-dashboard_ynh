
- download and extract sources, navigate to the dir then:
- `git init`
- `git add *`
- `find ./ \( -type d -name .git -prune \) -o -type f -print0 | xargs -0 sed -i 's/\/var\/lxdware/\/home\/yunohost.app\/lxd-dashboard/g'`
- `git diff > main-replace_data_dir.patch`