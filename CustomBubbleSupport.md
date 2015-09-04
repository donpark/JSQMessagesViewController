JSQMessagesCollectionViewDataSource.h

- (void)collectionView:(JSQMessagesCollectionView *)collectionView cell:(JSQMessagesCollectionViewCell *)cell applyStylesForItemIndexPath:(NSIndexPath *)indexPath;

JSQMessagesViewController.m

        if ([collectionView.dataSource respondsToSelector:@selector(collectionView:cell:applyStylesForItemIndexPath:)]) {
            [collectionView.dataSource collectionView:collectionView
                                                 cell:cell
                          applyStylesForItemIndexPath:indexPath];
        }
