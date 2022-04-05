# update_outdated_librabies
update libraries that are outdated


pip list --outdated --format=freeze | grep -v '^\-e' | cut -d = -f 1 | xargs -n1 pip install -U
