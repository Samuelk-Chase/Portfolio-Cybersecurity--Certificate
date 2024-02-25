# Updating "allow_list.txt" with Python Algorithm

## Project Description

    At my organization, access to restricted content is controlled with an allow list of IP addresses. The "allow_list.txt" file identifies these IP addresses. A separate remove list identifies IP addresses that should no longer have access to this content. I created an algorithm to automate updating the "allow_list.txt" file and remove these IP addresses that should no longer have access.


## Algorithm

    import_file = "allow_list.txt"

# Open the File
    with open(import_file, "r") as file:
        # Read the File Contents
        ip_addresses = file.read()

        # Convert the String into a List
        ip_addresses = ip_addresses.split()

        # Iterate through the Remove List
        for element in remove_list:
            # Remove IP Addresses from the Allow List
            if element in ip_addresses:
                ip_addresses.remove(element)

# Update the File
    with open(import_file, "w") as file:
        file.write("\n".join(ip_addresses))

## Summary
    This algorithm removes IP addresses identified in a `remove_list` variable from the "allow_list.txt" file of approved IP addresses. It involves opening the file, converting it to a string to be read, converting this string to a list, iterating through the IP addresses in `remove_list`, removing IP addresses from the allow list, and finally updating the file with the revised list of IP addresses.

