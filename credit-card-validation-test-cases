import unittest
from valid_card_checker import is_valid_card


class MyTest(unittest.TestCase):
    def test2(self):
        self.assertEqual(is_valid_card('4123456789123456'), 'Valid')
        self.assertEqual(is_valid_card('5123-4567-8912-3456'), 'Valid')
        self.assertEqual(is_valid_card('61234-567-8912-3456'), 'Invalid')
        self.assertEqual(is_valid_card('4123356789123456'), 'Valid')
        self.assertEqual(is_valid_card('5133-3367-8912-3456'), 'Invalid')
        self.assertEqual(is_valid_card('5123 - 3567 - 8912 - 3456'), 'Invalid')


if _name_ == '_main_':
    unittest.main()
