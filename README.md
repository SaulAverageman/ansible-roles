roles/<br>
    common/               # this hierarchy represents a "role"<br>
        tasks/            #<br>
            main.yml      #  <-- tasks file can include smaller files if warranted<br>
        handlers/         #<br>
            main.yml      #  <-- handlers file<br>
        templates/        #  <-- files for use with the template resource<br>
            ntp.conf.j2   #  <------- templates end in .j2<br>
        files/            #<br>
            bar.txt       #  <-- files for use with the copy resource<br>
            foo.sh        #  <-- script files for use with the script resource<br>
        vars/             #<br>
            main.yml      #  <-- variables associated with this role<br>
        defaults/         #<br>
            main.yml      #  <-- default lower priority variables for this role<br>
        meta/             #<br>
            main.yml      #  <-- role dependencies <br>
        library/          # roles can also include custom modules<br>
        module_utils/     # roles can also include custom module_utils<br>
        lookup_plugins/   # or other types of plugins, like lookup in this case<br>

    webtier/              # same kind of structure as "common" was above, done for the webtier role<br>
    monitoring/           # ""<br>
    fooapp/ <br>
