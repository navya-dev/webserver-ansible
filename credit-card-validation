import re


PATTERN=r"^(?!.*([0-9])(?:-?\1){3})[456][0-9]{3}(-?)[0-9]{4}\2[0-9]{4}\2[0-9]{4}$"


def is_valid_card(sequence):
    if re.search(PATTERN, sequence):
        print('Valid')
        return 'Valid'
    else:
        print('Invalid')
        return 'Invalid'

if _name_ == '_main_':
    cards = ['4123456789123456',
             '5123-4567-8912-3456',
             '61234-567-8912-3456',
             '4123356789123456',
             '5133-3367-8912-3456',
             '5123 - 3567 - 8912 - 3456'
             ]

    for card in cards:
        is_valid_card(card)
