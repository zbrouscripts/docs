# Permissions and administration

## Main owner

The owner has full access to FraseKill Admin.

Add one line to `server.cfg`:

```cfg
add_ace identifier.license:YOUR_LICENSE zbrou.frasekill.admin allow
```

If you do not know your license, join the server and run `/frasekilladmin`. FraseKill will show the exact line you need to copy.

## Add more administrators

You do not need more ACE lines.

The owner can create administrators from the panel and choose what each one can do, such as viewing players, managing access, editing/resetting FraseKill, managing rules and changing Script settings.

Being an administrator does **not** automatically give player access to FraseKill.

## Player access

Access can be permanent or limited to hours, days, weeks, months or years.

You can also grant access to jobs or groups.

For Tebex, see **Script settings → Access and Tebex**.
